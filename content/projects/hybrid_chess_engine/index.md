---
title: "Chess Engine Framework"
weight: 3
---

# Chess Engine Framework

*Built for a Warwick chess engine competition sponsored by Optiver · Dec 2025 – Jan 2026*

{{< tech >}}C++, Python, Numba, SFML{{< /tech >}}

[Framework on GitHub](https://github.com/edwardodp/chess-engine-framework) · [Competition starter repo](https://github.com/edwardodp/chess-engine-compeititon)

A chess engine platform where students write an evaluation function in Python and plug it into a shared C++ search. I organised the competition it was built for with the Warwick Computing Society and Chess Society: around 40 students entered, and the finalists' engines played rated human players live. I wrote the C++ engine (move generation, search and the GUI); Jakub Kisielewski built much of the Python tooling competitors worked with.

## Python evaluation at C++ speed

Competitors write a single evaluation function in Python, restricted to what Numba can compile. The framework compiles it with Numba's `@cfunc` into a native function pointer and passes that to the C++ library through `ctypes`, so the search calls it with no interpreter in the loop. Without that, crossing between Python and C++ at every node of the search would have made the engine orders of magnitude slower. A small dispatcher routes each call to the right bot, so two different evaluations can play each other through the same search.

## The search

The board is a set of bitboards, one 64-bit integer per piece type. On top of legal move generation, the search grew from plain minimax into negamax with alpha-beta pruning and principal variation search, with iterative deepening, quiescence search to mitigate the horizon effect, and move ordering (MVV-LVA for captures, killer moves and the history heuristic for quiet moves). Positions are Zobrist-hashed, and draws are detected by threefold repetition and the fifty-move rule. Because every competitor shared this search, the competition came down purely to who could evaluate a position best.

## Tooling

- An SFML GUI for human vs bot and bot vs bot games, with move highlighting, undo and PGN export.
- Headless round-robin tournaments run in parallel across processes, used to pick the finalists.
- Prebuilt libraries for Windows, Linux and both Mac architectures, built by GitHub Actions.

## The showdown

Three finalist bots each played humans rated roughly 2200, 1600 and 1000 (ECF). Searching to depth 7, the top-seeded student bot beat the 2200-rated player.
