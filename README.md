# Instruments for LLM / agent evaluation and reliability

This is a **profile README** (not a product). The public work lives in the named repos below — clone those, not this page.

## Projects

| Project | What it does |
| --- | --- |
| [judge-drift-sentinel](https://github.com/homayoun-safarpour/judge-drift-sentinel) | Eval score moved: was it the system or the LLM judge? Frozen anchors + CI exit codes. |
| [judge-reliability-kit](https://github.com/homayoun-safarpour/judge-reliability-kit) | Low panel kappa: item ambiguity vs rubric underspecification. |
| [agent-loop-engine](https://github.com/homayoun-safarpour/agent-loop-engine) | State → gates → decide → journal. Repair before advance. |
| [agent-loop-field-guide](https://github.com/homayoun-safarpour/agent-loop-field-guide) | Five-decision Loop Contract template before you automate. |
| [trace-gate](https://github.com/homayoun-safarpour/trace-gate) | Trajectory score vs frozen baseline; fail-closed deploy gate. |
| [rag-eval-service](https://github.com/homayoun-safarpour/rag-eval-service) | RAG ingest/query + frozen hit@k / MRR check. |
| [agent-eval-workbench](https://github.com/homayoun-safarpour/agent-eval-workbench) | Scenario traces + detectors; `--min-composite` exit 2. |
| [repro-ml-pipeline](https://github.com/homayoun-safarpour/repro-ml-pipeline) | Train → register → serve with a verified run signature. |
| [ai-eng-skill-range](https://github.com/homayoun-safarpour/ai-eng-skill-range) | 56 skills / 24 graded katas (`skillrange grade`, exit 0/2). |

Shared contract: Python 3.10–3.12 CI, named tests behind README claims, deterministic cores where the README says so. Sentinel and trace-gate speak exit `0`/`2` so agent-loop-engine can use them as gates.

## Start here

Pick one repo. Run the README Quickstart / worked example (under 30 minutes). Each ships fixtures in-repo; most have `docs/INTERVIEW.md` with CLI talking points.

## Links

- GitHub: [@homayoun-safarpour](https://github.com/homayoun-safarpour)
- LinkedIn: [homayoun-safarpour](https://www.linkedin.com/in/homayoun-safarpour/)
