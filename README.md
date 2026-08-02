# Homayoun Safarpour

**AI engineer. Evaluation, reliability, and trust for LLM and agent systems.**

I build production-facing instruments for when machines judge: disagreement diagnosis, judge-drift attribution, deterministic agent loops, and CI gates with exit codes you can wire into pipelines. One public ship per week, daily commits, tests + CI on Python 3.10–3.12 from commit one. Every README claim is backed by a named test. Deterministic cores; zero LLM dependency in the measurement path.

## Shipping daily

**This week: [judge-drift-sentinel](https://github.com/homayoun-safarpour/judge-drift-sentinel).**
When eval scores move, it tells you whether your system changed or your LLM judge did, by re-scoring a frozen human-labeled anchor set and comparing agreement against the pinned baseline. Deterministic core, no LLM dependency, exit codes built for CI gates.

Also live:

- [judge-reliability-kit](https://github.com/homayoun-safarpour/judge-reliability-kit): a low kappa says your judge panel is broken; this decomposes *why* (item ambiguity vs rubric underspecification), so you fix the right thing.
- [agent-loop-engine](https://github.com/homayoun-safarpour/agent-loop-engine): a self-advancing agent loop with markdown state, quality gates, a deterministic three-rule decision policy, and an append-only journal, so agent behavior is auditable instead of anecdotal.
- [trace-gate](https://github.com/homayoun-safarpour/trace-gate): gates a deploy on agent trajectory scores pinned to a frozen baseline (exit 0/2), so tool-use regressions fail CI the same way unit tests do.
- [rag-eval-service](https://github.com/homayoun-safarpour/rag-eval-service): FastAPI RAG evaluation with hit@k / MRR and a frozen-metric regression gate (`corpus_sha256`), so corpus edits cannot hide under old numbers.
- [agent-eval-workbench](https://github.com/homayoun-safarpour/agent-eval-workbench): multi-axis agent scorecard (task success, reliability, bias gap, named failure modes) with `--min-composite` exit 2.
- [repro-ml-pipeline](https://github.com/homayoun-safarpour/repro-ml-pipeline): sklearn + MLflow training with a data/params signature hash verified in CI.

## Fork these first

Each repo is meant to be cloned and run in under 30 minutes. Start with the worked example, not the source tree.

| Repo | Clone and run | Fixture data already in-repo |
| --- | --- | --- |
| [judge-reliability-kit](https://github.com/homayoun-safarpour/judge-reliability-kit) | `examples/worked_example.py` | `examples/judge_panel_ratings.json` |
| [judge-drift-sentinel](https://github.com/homayoun-safarpour/judge-drift-sentinel) | README Quickstart (`baseline` / `check`) | `examples/anchors.jsonl`, `examples/run_*.json` |
| [agent-loop-engine](https://github.com/homayoun-safarpour/agent-loop-engine) | README Quickstart on `examples/LOOP_STATE.md` | `examples/LOOP_STATE.md`, `examples/journal/` |
| [trace-gate](https://github.com/homayoun-safarpour/trace-gate) | README Quickstart (`freeze` / `check`) | `examples/trajectories/`, `examples/rubric.json` |
| [rag-eval-service](https://github.com/homayoun-safarpour/rag-eval-service) | README Quickstart (`evaluate` / `check`) | `examples/corpus.json`, `examples/cases.json`, `examples/baseline_v1.json` |
| [agent-eval-workbench](https://github.com/homayoun-safarpour/agent-eval-workbench) | README Quickstart (`score`) | `examples/bundle_*.json`, `examples/scorecard_mixed.json` |
| [repro-ml-pipeline](https://github.com/homayoun-safarpour/repro-ml-pipeline) | README Quickstart (`train` / `verify-signature`) | `examples/artifacts/run_signature.json`, `examples/train_summary.json` |

Stack wiring: sentinel and trace-gate speak exit `0`/`2` so [agent-loop-engine](https://github.com/homayoun-safarpour/agent-loop-engine) can treat them as quality gates. Kit panel exports feed the sentinel adapter.

## What I'm building against

- **LLM-judge drift is a named 2026 failure mode with prescribed but un-toolified ops**
  (pin the judge, keep a frozen anchor set, track kappa on a cadence; field guidance from
  futureagi.com and llmtrace.io, surveyed 2026-08-03). → judge-drift-sentinel implements
  that ops loop as a CLI.
- **Evals and observability top the hiring gap**: observability appears in 42% and CI/CD in
  33.9% of 43k AI-engineering postings (axialsearch.com, read 2026-08-03); evaluation is
  called the top gap to close (axialsearch.com, read 2026-08-03). → judge-reliability-kit and judge-drift-sentinel
  are evaluation infrastructure; every repo wires into CI.
- **Constraint drift in long-horizon agents is measured but un-toolified**: DRIFT-Bench
  reports 3.4x constraint-violation growth across task quartiles (2026 benchmark, surveyed
  2026-08-03). → agent-loop-engine's append-only journal makes agent behavior auditable;
  a constraint-decay auditor on top of it is next on the roadmap.
- **Context engineering has replaced prompt engineering as the production-agent skill**
  ("context rot", ICML 2026 agentic workshop slate; surveyed 2026-08-03). → a context-window
  ledger (what is in the window, what each block costs, what to evict) follows on the
  same roadmap.

## Capabilities

| area | evidence |
| --- | --- |
| Evaluation & measurement | Agreement statistics (Cohen/Fleiss kappa), frozen anchor sets, drift attribution, decomposition of disagreement into actionable causes |
| Agentic systems | Deterministic decision policies, quality gates, append-only state, loops that advance themselves and leave an audit trail |
| Engineering rigor | Tests + ruff + GitHub Actions CI (Python 3.10/3.11/3.12) on every repo from commit #1; every README claim has a named test; worked examples run for real |

## Contact

- GitHub: [@homayoun-safarpour](https://github.com/homayoun-safarpour)
- LinkedIn: [homayoun-safarpour](https://www.linkedin.com/in/homayoun-safarpour/)
