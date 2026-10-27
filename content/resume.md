---
title: "Resume"
---

# Edward O'Dwyer

{{< email user="edward.o-dwyer" domain="warwick.ac.uk" display="edward (dot) o-dwyer [at] warwick.ac.uk" >}} · [in/edward-odwyer](https://linkedin.com/in/edward-odwyer) · [github.com/edwardodp](https://github.com/edwardodp)

---

## Technical Skills

**Languages:** Java, Python, C/C++, SQL (PostgreSQL & SQLite), Shell script, Haskell

**Dev. Tools/Frameworks:** Git/GitHub, Linux/UNIX, Neovim, Valgrind, ASan/UBSan, Maven, JUnit, NumPy, Pandas, REST

**Concepts:** Low-Latency Systems, Concurrency, API Design, Distributed Systems

---

## Education

{{< entry title="University of Warwick" date="Sep 2024 – Jul 2027 · Coventry, UK" >}}

*Bachelor of Science (Honours) in Computer Science*
- Expected: First
- Modules: Compiler Design, High Performance Computing (4th-year module)
- Dissertation: *eDSL for Compile-Time Task Dependency Graph Optimisation* (C++)

{{< entry title="The American School in London" date="Aug 2017 – Jun 2024 · London, UK" >}}

*High School Diploma*

---

## Experience

{{< entry title="Data Engineer Intern @ Homey Technology" date="Jul 2025 – Sep 2025 · London, UK" >}}

{{< tech >}}Python, Pandas, NumPy, Plotly, Streamlit, PostHog, PostgreSQL{{< /tech >}}

- Drove a {{< num >}}97%{{< /num >}} {{< bright >}}reduction in KPI dashboard latency{{< /bright >}} via a {{< bright >}}concurrent caching system{{< /bright >}} with per-query mutex locks
- Built a {{< bright >}}company-wide KPI dashboard{{< /bright >}} unifying {{< num >}}5{{< /num >}} data sources, architected so new sources plug in easily
- Applied {{< bright >}}correlation analysis{{< /bright >}} and lines of best fit to KPI trends, producing {{< num >}}20+{{< /num >}} {{< bright >}}strategic forecasts{{< /bright >}}

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
- Implemented {{< bright >}}Spatial Partitioning{{< /bright >}} via Cell Lists to optimise collision detection from **O(N²) to O(N)** ensuring performance
- Developed a {{< bright >}}Monte Carlo Search algorithm{{< /bright >}} to optimise barrier placement, achieving a {{< num >}}~60%{{< /num >}} reduction in crowd pressure

{{< entry title="Hybrid Chess Engine Framework" date="Dec 2025 – Jan 2026" >}}

{{< tech >}}C++, Python, Numba, SFML{{< /tech >}}

- Designed a hybrid engine letting users inject {{< bright >}}Numba-compiled machine code{{< /bright >}} into a low-latency C++ backend
- Evolved search from Minimax to {{< bright >}}Negamax with Alpha-Beta pruning{{< /bright >}}, adding {{< bright >}}Quiescence Search{{< /bright >}} to mitigate the horizon effect
- Built move generation and GUI from scratch in {{< bright >}}C++ and SFML{{< /bright >}}, using {{< bright >}}bitboards{{< /bright >}} for fast validation within {{< num >}}150{{< /num >}}MB of memory

{{< entry title="Network Attacks Identifier" date="Nov 2025 – Dec 2025" >}}

{{< tech >}}C, POSIX Threads{{< /tech >}}

- Architected a {{< bright >}}single-producer, multi-consumer{{< /bright >}} pipeline with a worker pool sized to core count for true parallelism
- Engineered a lock-synced {{< bright >}}ring buffer{{< /bright >}} for passing packets, eliminating per-packet allocation and exploiting cache locality
- Applied {{< bright >}}fine-grained locking{{< /bright >}} over shared detection state, verifying {{< bright >}}memory safety{{< /bright >}} under attack simulation with Valgrind

{{< entry title="A=B Esolang Interpreter" date="Mar 2025 – Apr 2025" >}}

{{< tech >}}Haskell, Cabal, Stack{{< /tech >}}

- Built an {{< bright >}}interpreter{{< /bright >}} for the A=B (a to b) esoteric language using Haskell, featuring a {{< bright >}}custom parser{{< /bright >}}
- Achieved correct interpretation of {{< num >}}100%{{< /num >}} of official A=B examples, demonstrating deep understanding of idiomatic Haskell

---

## Awards

{{< entry title="UKIEPC 2026 – 2nd of 22 Warwick Teams" date="Oct 2026" >}}

- Competed in the {{< bright >}}UK & Ireland Programming Contest{{< /bright >}}, an ICPC-format algorithmic competition for university teams

{{< entry title="IC Algothon 24 – Finalist" date="Nov 2024" >}}

{{< tech >}}Python, NumPy, Pandas, Matplotlib, JavaScript{{< /tech >}}

- Placed {{< num >}}9th{{< /num >}} out of {{< num >}}~200{{< /num >}} teams (top {{< num >}}4.5%{{< /num >}}) in {{< bright >}}Europe's largest algorithmic trading hackathon{{< /bright >}} ({{< num >}}25%{{< /num >}} admittance rate)

---

## Leadership

{{< entry title="Warwick Hackathon Organiser @ WHACK" date="Oct 2024 – Present" >}}

- Co-lead organiser of {{< bright >}}WHACK 2026{{< /bright >}}: tripled sponsorship to £{{< num >}}30k{{< /num >}} and doubled capacity to {{< num >}}400{{< /num >}} year-on-year
- Owned sponsor negotiations end-to-end, restructuring tiers around a £{{< num >}}10k{{< /num >}} {{< bright >}}title package{{< /bright >}} to anchor gold pricing
- Built a {{< bright >}}Binomial turnout model{{< /bright >}} with a CLT approximation to size overbooking: {{< num >}}521{{< /num >}} places at {{< num >}}0.1%{{< /num >}} overflow risk

{{< entry title="Academic Executive Officer @ University of Warwick Computing Society" date="Oct 2024 – Jun 2026" >}}

- Supported dozens of students through recruitment with resume reviews, mock interviews, resources and workshops
- Partnered with {{< num >}}10+{{< /num >}} societies on {{< bright >}}joint events{{< /bright >}}, reaching compromises through responsive, needs-focused collaboration
- Led a {{< bright >}}Chess Engine Competition{{< /bright >}} for {{< num >}}40{{< /num >}} competitors, securing Optiver as sponsor and building the framework it ran on
