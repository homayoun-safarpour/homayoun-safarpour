# Homayoun

**Eval score moved. You cannot tell whether the system regressed or the judge did.**

judge-drift-sentinel · judge-reliability-kit · agent-loop-engine · trace-gate · ai-eng-skill-range

```bash
pip install judge-drift-sentinel
git clone https://github.com/homayoun-safarpour/judge-drift-sentinel
cd judge-drift-sentinel
drift-sentinel check --anchors examples/anchors.jsonl --baseline examples/run_baseline.json --current examples/run_current.json
```

```text
verdict      : JUDGE_DRIFT
anchor kappa : 0.833 -> 0.333
anchor flips : 25.0% of frozen anchors changed label
judge pin    : CHANGED frontier-4-2026-05-01@9f2c1a -> frontier-4-latest@9f2c1a
live metric  : moved -0.150
reason       : agreement with the frozen human labels fell (0.833 -> 0.333); the ruler moved, not the system
```

That command exits 2. Clone a named project below, not this profile repo.

## Projects

| Project | Job |
| --- | --- |
| [judge-drift-sentinel](https://github.com/homayoun-safarpour/judge-drift-sentinel) | Score moved: system or LLM judge? |
| [judge-reliability-kit](https://github.com/homayoun-safarpour/judge-reliability-kit) | Why a judge panel disagrees (kappa) |
| [agent-loop-engine](https://github.com/homayoun-safarpour/agent-loop-engine) | State, gates, decide, journal |
| [agent-loop-field-guide](https://github.com/homayoun-safarpour/agent-loop-field-guide) | Loop Contract before you automate |
| [trace-gate](https://github.com/homayoun-safarpour/trace-gate) | Trajectory deploy gate (exit 0/2) |
| [rag-eval-service](https://github.com/homayoun-safarpour/rag-eval-service) | RAG path + frozen hit@k / MRR |
| [agent-eval-workbench](https://github.com/homayoun-safarpour/agent-eval-workbench) | Scenario traces + detectors |
| [repro-ml-pipeline](https://github.com/homayoun-safarpour/repro-ml-pipeline) | Train, register, serve + signature |
| [ai-eng-skill-range](https://github.com/homayoun-safarpour/ai-eng-skill-range) | 56 skills / 24 graded katas |
| [agent-constraint-auditor](https://github.com/homayoun-safarpour/agent-constraint-auditor) | Audit agent transcripts for declared-constraint decay |
| [judge-field-guide](https://github.com/homayoun-safarpour/judge-field-guide) | Link-checked map of the judge tool ecosystem |

Python 3.10-3.12 CI. Named tests behind README claims. Quickstart under 30 minutes.

## Links

- [@homayoun-safarpour](https://github.com/homayoun-safarpour)
- [LinkedIn](https://www.linkedin.com/in/homayoun-safarpour/)
