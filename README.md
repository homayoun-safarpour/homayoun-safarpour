# Evaluation, reliability, and trust for LLM and agent systems

**Homayoun Safarpour** — AI engineer. Open instruments for when machines judge: deterministic cores, CI exit codes, named tests on every README claim (Python 3.10–3.12).

## Instruments

| Pain | Repo |
| --- | --- |
| Eval scores moved after a model swap — is it your system or judge drift? | [judge-drift-sentinel](https://github.com/homayoun-safarpour/judge-drift-sentinel) |
| Low kappa on the judge panel — rubric or item ambiguity? | [judge-reliability-kit](https://github.com/homayoun-safarpour/judge-reliability-kit) |
| Agent keeps shipping while gates are red — need repair-before-advance | [agent-loop-engine](https://github.com/homayoun-safarpour/agent-loop-engine) |
| Need graded, exit-code katas an org or bot can score | [ai-eng-skill-range](https://github.com/homayoun-safarpour/ai-eng-skill-range) |

Each repo includes a worked example (clone → run in under 30 minutes) and **`docs/INTERVIEW.md`** — design choices, failure modes, and how to demo it in a technical conversation.

More live tools: [trace-gate](https://github.com/homayoun-safarpour/trace-gate) (trajectory CI gates), [rag-eval-service](https://github.com/homayoun-safarpour/rag-eval-service) (frozen RAG hit@k/MRR), [agent-eval-workbench](https://github.com/homayoun-safarpour/agent-eval-workbench) (YAML scenarios + trace detectors), [agent-loop-field-guide](https://github.com/homayoun-safarpour/agent-loop-field-guide) (loop contract templates), [repro-ml-pipeline](https://github.com/homayoun-safarpour/repro-ml-pipeline) (train → serve signature verify).

Sentinel and trace-gate use exit `0`/`2` so agent-loop-engine can wire them as quality gates; kit panel exports feed the sentinel adapter.

## Contact

- GitHub: [@homayoun-safarpour](https://github.com/homayoun-safarpour)
- LinkedIn: [homayoun-safarpour](https://www.linkedin.com/in/homayoun-safarpour/)