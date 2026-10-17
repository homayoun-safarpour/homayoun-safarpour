# Homayoun Safarpour

I build Python tools for agent reliability, LLM evaluation, and reproducible ML.

My focus is **fail-closed checks**: explicit pass/fail signals, frozen baselines, and evidence you can inspect. A green CI run should mean the checks actually ran.

## Agent reliability

| Project | What it does |
| --- | --- |
| [homi-gate](https://github.com/homayoun-safarpour/homi-gate) | Checks completion, handoffs, MCP tool-access configuration, tool calls, and trajectories |
| [trace-gate](https://github.com/homayoun-safarpour/trace-gate) | Gates trajectory regressions against a frozen baseline and pinned rubric |
| [judge-drift-sentinel](https://github.com/homayoun-safarpour/judge-drift-sentinel) | Tracks judge agreement with frozen human anchors across runs |
| [agent-constraint-auditor](https://github.com/homayoun-safarpour/agent-constraint-auditor) | Audits transcripts against declared regex constraints |
| [agent-loop-engine](https://github.com/homayoun-safarpour/agent-loop-engine) | Chooses one bounded next action from state and quality gates, then journals the decision |

Start with **homi-gate** for run and handoff checks, **trace-gate** for trajectory regressions, or **judge-drift-sentinel** when judge scores move.

## Evaluation and ML

| Project | What it does |
| --- | --- |
| [judge-reliability-kit](https://github.com/homayoun-safarpour/judge-reliability-kit) | Measures judge agreement and repeated-rating consistency to diagnose disagreement |
| [agent-eval-workbench](https://github.com/homayoun-safarpour/agent-eval-workbench) | Runs scenario-based evaluations with trace-derived failure detectors |
| [rag-eval-service](https://github.com/homayoun-safarpour/rag-eval-service) | Checks retrieval metrics against frozen hit@k and MRR baselines |
| [repro-ml-pipeline](https://github.com/homayoun-safarpour/repro-ml-pipeline) | Connects scikit-learn, MLflow, and FastAPI with a locked environment and run-signature checks |

## Guides and practice

- [ai-eng-skill-range](https://github.com/homayoun-safarpour/ai-eng-skill-range): offline engineering exercises with pass/fail graders
- [agent-loop-field-guide](https://github.com/homayoun-safarpour/agent-loop-field-guide): a five-decision Loop Contract, templates, and a heading checker
- [judge-field-guide](https://github.com/homayoun-safarpour/judge-field-guide): a curated judge-tool registry with schema and link checks

## How I work

- Start with a concrete failure mode
- Show passing and failing examples
- Make criteria, baselines, and exit codes explicit
- Document limits and how each tool fits alongside other systems

Open a project above for its quickstart, tests, and limitations. Setup differs by project; this repository is the profile index.

## Links

- [GitHub](https://github.com/homayoun-safarpour)
- [LinkedIn](https://www.linkedin.com/in/homayoun-safarpour/)
- [ORCID: 0000-0002-3206-5357](https://orcid.org/0000-0002-3206-5357)
