---
title: "Network Attacks Identifier"
weight: 4
---

# Network Attacks Identifier

*Operating systems and networks coursework · Nov – Dec 2025*

{{< tech >}}C, POSIX Threads{{< /tech >}}

A multi-threaded program that captures live network traffic and analyses every packet for signs of malicious activity. It's university coursework, so the code isn't public; this is a summary of the design from my report. The detection rules were set by the brief. What interested me was the systems problem underneath: making analysis keep up with capture.

## Two goals

Capture has to be fast, because a slow sniffer drops packets. Analysis is far more expensive than capture, so it has to keep pace, or the backlog of unanalysed packets grows without bound. Every decision below follows from those two.

## One producer, many consumers

A single capture thread produces packets, and a pool of analysis workers consumes them. The pool is sized to the number of cores: analysis is CPU-bound with no blocking I/O, so any extra threads would only add context switches. The workers live for the whole run rather than being created per packet, and a condition variable wakes a sleeping worker when work arrives.

## Ring buffer over linked list

A linked-list queue can grow as large as memory allows, but it costs an allocation per packet and scatters packets across the heap. A fixed-size ring buffer needs no allocation at all and keeps packets contiguous, which the cache rewards. The trade-off is that a full backlog arrives sooner. For a capture path where speed matters more than memory, that's the right trade.

## Locking

- The queue is protected by a mutex. Modern mutexes spin briefly before putting a thread to sleep, which suits both bursts of traffic and quiet periods.
- Detection statistics are split into independent sections with a lock each, so two workers recording different kinds of event never block each other.

## Shutdown and memory safety

On Ctrl-C, capture stops and the workers drain anything still queued, so no captured packet goes unanalysed, before the threads are joined and resources are freed in order. I tested under Valgrind, including running two attack simulations at once from a bash script, and found no leaks.
