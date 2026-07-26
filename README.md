# Homayoun Safarpour

**AI engineer specializing in machines that judge — evaluation, reliability, and trust for LLM systems.**

I ship one public project per week, one commit per day minimum. Every repo has tests, CI on
three Python versions, and a README where every claim is backed by a named test.

## Shipping daily

**This week: [judge-drift-sentinel](https://github.com/homayoun-safarpour/judge-drift-sentinel)** —
when your eval scores move, it tells you whether your system changed or your LLM judge did,
by re-scoring a frozen human-labeled anchor set and comparing agreement against the pinned
baseline. Deterministic core, no LLM dependency, exit codes built for CI gates.

Also live:

- [judge-reliability-kit](https://github.com/homayoun-safarpour/judge-reliability-kit) — a low
  kappa says your judge panel is broken; this decomposes *why* (item ambiguity vs rubric
  underspecification), so you fix the right thing.
- [agent-loop-engine](https://github.com/homayoun-safarpour/agent-loop-engine) — a
  self-advancing agent loop: markdown state, quality gates, a deterministic three-rule decision
  policy, and an append-only journal, so agent behavior is auditable instead of anecdotal.

## Market trends I'm building against

- **LLM-judge drift is a named 2026 failure mode with prescribed but un-toolified practice**
  (pin the judge, keep a frozen anchor set, track kappa on a cadence — field guidance from
  futureagi.com and llmtrace.io, surveyed 2026-08-03). → judge-drift-sentinel implements
  exactly that practice as a CLI.
- **Evals and observability top the hiring gap**: observability appears in 42% and CI/CD in
  33.9% of 43k AI-engineering postings (axialsearch.com, read 2026-08-03); evaluation is
  called "the highest-leverage gap to close". → judge-reliability-kit and judge-drift-sentinel
  are evaluation infrastructure; every repo wires into CI.
- **Constraint drift in long-horizon agents is measured but un-toolified**: DRIFT-Bench
  reports 3.4x constraint-violation growth across task quartiles (2026 benchmark, surveyed
  2026-08-03). → agent-loop-engine's append-only journal makes agent behavior auditable;
  a constraint-decay auditor on top of it is next on the roadmap.
- **Context engineering has replaced prompt engineering as the production-agent skill**
  ("context rot", ICML 2026 agentic workshop slate; surveyed 2026-08-03). → a context-window
  ledger — what is in the window, what each block costs, what to evict — follows on the
  same roadmap.

## Capabilities

| area | evidence |
| --- | --- |
| Evaluation & measurement | Agreement statistics (Cohen/Fleiss kappa), frozen anchor sets, drift attribution, decomposition of disagreement into actionable causes |
| Agentic systems | Deterministic decision policies, quality gates, append-only state, loops that advance themselves and leave an audit trail |
| Engineering rigor | Tests + ruff + GitHub Actions CI (Python 3.10/3.11/3.12) on every repo from commit #1; every README claim has a named test; worked examples run for real |

## Contact

- GitHub: [@homayoun-safarpour](https://github.com/homayoun-safarpour)
- LinkedIn: _add your LinkedIn URL here_
