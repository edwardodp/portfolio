---
title: "Resume"
---

# Edward O'Dwyer

{{< email user="edward.o-dwyer" domain="warwick.ac.uk" display="edward (dot) o-dwyer [at] warwick.ac.uk" >}} · [in/edward-odwyer](https://linkedin.com/in/edward-odwyer) · [github.com/edwardodp](https://github.com/edwardodp)

---

## Education

{{< entry title="University of Warwick" date="Sep 2024 – Jul 2027 · Coventry, UK" >}}

*Bachelor of Science (Honours) in Computer Science*
- Expected: First
- Modules: Advanced Computer Architecture, Compilers, High Performance Computing (4th-year module)
- Dissertation: *eDSL for Compile-Time Task Dependency Graph Optimisation* (C++)

{{< entry title="The American School in London" date="Aug 2017 – Jun 2024 · London, UK" >}}

*High School Diploma*

---

## Awards

{{< entry title="QRT C3 Hackathon 2026 – 2nd of 64 Teams" date="Qualified for Inter-University Final · Nov 2026" >}}

- Owned the packing problem ({{< num >}}5th{{< /num >}} of {{< num >}}64{{< /num >}}), split across exact search, {{< bright >}}CP-SAT{{< /bright >}} and heuristics: {{< num >}}34%{{< /num >}} proven optimal
- Ran each method as an {{< bright >}}AI coding agent{{< /bright >}} in a sandboxed environment I built, moving CPU to whatever was paying off

{{< entry title="UKIEPC 2026 – 2nd of 22 Warwick Teams" date="Qualified for NWERC · Oct 2026" >}}

- Competed in the {{< bright >}}UK & Ireland Programming Contest{{< /bright >}}, an ICPC-format algorithmic competition for university teams

{{< entry title="IC Algothon 24 – Finalist" date="Nov 2024" >}}

{{< tech >}}Python, NumPy, Pandas, Matplotlib, JavaScript{{< /tech >}}

- Placed {{< num >}}9th{{< /num >}} out of {{< num >}}~200{{< /num >}} teams (top {{< num >}}4.5%{{< /num >}}) in {{< bright >}}Europe's largest algorithmic trading hackathon{{< /bright >}} ({{< num >}}25%{{< /num >}} admittance rate)

---

## Experience

{{< entry title="Data Engineer Intern @ Homey Technology" date="Jul 2025 – Sep 2025 · London, UK" >}}

{{< tech >}}Python, Pandas, NumPy, Plotly, Streamlit, PostHog, PostgreSQL{{< /tech >}}

- Cut dashboard load times from {{< num >}}3s+{{< /num >}} to {{< num >}}~100ms{{< /num >}} with a {{< bright >}}concurrent cache{{< /bright >}}; per-query locks let charts load in parallel
- Cached historical data long-term and same-day data on a {{< num >}}5{{< /num >}}-minute {{< bright >}}TTL{{< /bright >}}, removing the need for a costly ETL pipeline
- Architected a backend unifying {{< num >}}5{{< /num >}} {{< bright >}}data sources{{< /bright >}} behind one interface, so new sources plug in easily

---

## Projects

{{< entry title="Airport Traffic Simulation" date="Departmental Prize · Jan 2026 – Mar 2026" >}}

{{< tech >}}Java, JavaFX, Maven, JUnit{{< /tech >}}

- Architected the {{< bright >}}MVVM{{< /bright >}} design for a team of {{< num >}}6{{< /num >}}, using immutable state snapshots to decouple engine and UI
- Built the simulation engine's {{< bright >}}lock-free{{< /bright >}} threading model using AtomicReference and a concurrent command queue
- Implemented a {{< bright >}}headless mode{{< /bright >}} that skips snapshot allocation and rendering, running {{< num >}}720{{< /num >}} simulated hours in {{< num >}}0.3s{{< /num >}}

{{< entry title="Crowd Dynamics and Optimisation Engine" date="Built in 24h · Feb 2026" >}}

{{< tech >}}Python, Numba, NumPy{{< /tech >}}

- Engineered a custom {{< bright >}}Verlet integration physics engine{{< /bright >}}, utilising {{< bright >}}JIT compilation{{< /bright >}} to simulate {{< num >}}2,000+{{< /num >}} agents at {{< num >}}60{{< /num >}} FPS
- Implemented {{< bright >}}spatial partitioning{{< /bright >}} via cell lists, cutting collision detection from **O(N²) to O(N)**
- Developed a {{< bright >}}Monte Carlo Search algorithm{{< /bright >}} to optimise barrier placement, achieving a {{< num >}}~60%{{< /num >}} reduction in crowd pressure

{{< entry title="Hybrid Chess Engine Framework" date="Dec 2025 – Jan 2026" >}}

{{< tech >}}C++, Python, Numba, SFML{{< /tech >}}

- Designed a hybrid engine where competitors' Python evaluations compile via {{< bright >}}Numba{{< /bright >}} into native code for the C++ search
- Wrote an {{< bright >}}alpha-beta search{{< /bright >}} (PVS, quiescence, move ordering) that beat a {{< num >}}~2200{{< /num >}} ECF player with a competitor's evaluation
- Built {{< bright >}}magic-bitboard{{< /bright >}} move generation, exact on all {{< num >}}6{{< /num >}} standard perft positions at {{< num >}}57M{{< /num >}} positions/s

{{< entry title="Network Attacks Identifier" date="Nov 2025 – Dec 2025" >}}

{{< tech >}}C, POSIX Threads{{< /tech >}}

- Architected a {{< bright >}}single-producer, multi-consumer{{< /bright >}} pipeline with a worker pool sized to core count for true parallelism
- Engineered a lock-synced {{< bright >}}ring buffer{{< /bright >}} for passing packets, eliminating per-packet allocation and exploiting cache locality
- Applied {{< bright >}}fine-grained locking{{< /bright >}} over shared detection state, verifying {{< bright >}}memory safety{{< /bright >}} under attack simulation with Valgrind

{{< entry title="A=B Esolang Interpreter" date="Mar 2025 – Apr 2025" >}}

{{< tech >}}Haskell, Cabal, Stack{{< /tech >}}

- Built an {{< bright >}}interpreter{{< /bright >}} for the A=B esoteric language in Haskell, with a {{< bright >}}Megaparsec{{< /bright >}} parser-combinator front end
- Passes {{< num >}}100%{{< /num >}} of the official A=B examples, and extends the language so `(once)` combines with `(start)` and `(end)`

---

## Leadership

{{< entry title="Warwick Hackathon Organiser @ WHACK" date="Oct 2024 – Present" >}}

- Co-lead organiser of {{< bright >}}WHACK 2026{{< /bright >}}: nearly tripled sponsorship to £{{< num >}}26k{{< /num >}} and doubled capacity to {{< num >}}400{{< /num >}} year-on-year
- Owned sponsor negotiations end-to-end, restructuring tiers around a £{{< num >}}10k{{< /num >}} {{< bright >}}title package{{< /bright >}} to anchor gold pricing
- Built a {{< bright >}}Binomial turnout model{{< /bright >}} with a CLT approximation to size overbooking: {{< num >}}521{{< /num >}} places at {{< num >}}0.1%{{< /num >}} overflow risk

{{< entry title="Academic Executive Officer @ University of Warwick Computing Society" date="Oct 2024 – Jun 2026" >}}

- Supported {{< num >}}50+{{< /num >}} students through recruitment with CV reviews, mock interviews, resources and workshops
- Ran events with sponsors and {{< num >}}10+{{< /num >}} societies, reaching {{< num >}}1,000+{{< /num >}} attendees in total
- Led a {{< bright >}}Chess Engine Competition{{< /bright >}} for {{< num >}}40{{< /num >}} competitors, securing Optiver as sponsor and building the engine it ran on

---

## Technical Skills

**Languages:** Java, Python, C/C++, SQL (PostgreSQL & SQLite), Shell script, Haskell

**Dev. Tools/Frameworks:** Git/GitHub, Linux/UNIX, Neovim, Valgrind, ASan/UBSan, Maven, JUnit, NumPy, Pandas, REST

**Concepts:** Low-Latency Systems, Concurrency, API Design, Parallel Computing
