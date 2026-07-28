# deterministic-evals

> **A small research program with one rule: publish a result only where a
> deterministic oracle can score it.** No LLM judges, no vibes — a typecheck, a test,
> a known number, or nothing. Each study below states its hypothesis and protocol
> *before* the data, and reports the result whichever way it lands.

The throughline: an LLM "review" produces an opinion; an exit code produces a fact.
Everything here is built on the second kind.

## The studies

| Study | Claim (in one line) | Status |
|---|---|:---|
| **[gate-on-the-fact](https://github.com/NovemberFalls/gate-on-the-fact)** | A reviewer persona is theater; gate on a deterministic check, not an LLM judge. | **✅ Confirmed (placebo-controlled, saturating)** |
| **[capability-isnt-free](https://github.com/NovemberFalls/capability-isnt-free)** | Capability is not monotonic — an over-capable model is *worse* at mechanical work; route by verified accounting, not token price. | **🔬 Pre-registered, data pending** |
| **[cheapest-hands](https://github.com/NovemberFalls/cheapest-hands)** | Once the spec lowers a task to application, cheap/local hands clear the gate at a fraction of frontier cost. | **📊 Partial — powered run pending** |

Each status is a promise, not a boast: the confirmed one survived a pre-registered
protocol at k=25; the pending ones publish their hypothesis and method now and fill in
the result when the runs complete.

## The instrument

All three studies measure the same object: **[swarmsmith](https://github.com/NovemberFalls/swarmsmith)**,
an orchestration harness (the skills, agents, and deterministic gate that lower a task
to application so cheap hands can execute it). The studies cite it at a **pinned
version** as their data source — the instrument churns; the findings are frozen.

## Charts

Interactive charts, every losing run shown: **[boord-its.com/skills](https://boord-its.com/skills)**.

## Method, in one paragraph

Every claim is scored by a **hidden answer key** — a grading script the system under
test never sees, copied into a frozen test project only *after* a run ends. Oracles are
deterministic (planted bugs, exit-code checks, per-requirement partial credit). Fixtures
and answer keys are held private by design (an open answer key stops being hidden); the
methodology, oracle design, and gate setup are fully disclosed — enough to reproduce the
*shape* of any result on your own substrate.

## Built by

**November Falls.** MIT.
