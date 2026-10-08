# Homayoun Safarpour

**Agent CI stays green while the run is truncated, the handoff is `null`, or the MCP surface is wide open.**

I build **fail-closed gates** for agent / judge / RAG systems — deterministic exit codes, frozen anchors, no vibe scores.

Trustworthy AI / agentic systems · hire-facing OSS

```bash
pip install -e ".[dev]"   # in any gate repo below
homi-gate check-completion examples/pass.json
homi-gate check-handoff examples/handoff_ok.json
homi-gate check-mcp-allowlist examples/mcp_ok.yaml
```

Clone a **named project** below — not this profile repo.

## Gate stack (start here)

| Repo | Job | Fail signal |
|------|-----|-------------|
| [homi-gate](https://github.com/homayoun-safarpour/homi-gate) | Completion · handoff · MCP allowlist | exit `1` |
| [trace-gate](https://github.com/homayoun-safarpour/trace-gate) | Trajectory vs frozen baseline | exit `2` |
| [judge-drift-sentinel](https://github.com/homayoun-safarpour/judge-drift-sentinel) | Score moved: system or judge? | exit `2` |
| [agent-constraint-auditor](https://github.com/homayoun-safarpour/agent-constraint-auditor) | Declared-constraint decay in transcripts | exit `2` |
| [agent-loop-engine](https://github.com/homayoun-safarpour/agent-loop-engine) | State · gates · one action · journal | bounded loop |

## Eval & hire labs

| Repo | Job |
|------|-----|
| [judge-reliability-kit](https://github.com/homayoun-safarpour/judge-reliability-kit) | Why a judge panel disagrees (κ) |
| [agent-eval-workbench](https://github.com/homayoun-safarpour/agent-eval-workbench) | Scenario traces + detectors |
| [rag-eval-service](https://github.com/homayoun-safarpour/rag-eval-service) | Frozen RAG hit@k / MRR gates |
| [ai-eng-skill-range](https://github.com/homayoun-safarpour/ai-eng-skill-range) | 56 skills / 24 graded katas |
| [agent-loop-field-guide](https://github.com/homayoun-safarpour/agent-loop-field-guide) | Loop Contract before you automate |
| [judge-field-guide](https://github.com/homayoun-safarpour/judge-field-guide) | Link-checked judge-tool map |
| [repro-ml-pipeline](https://github.com/homayoun-safarpour/repro-ml-pipeline) | sklearn → MLflow → FastAPI + signature CI |

## How I ship (house style)

1. Lead with the **failure mode**, not the stack  
2. Pass + fail demo in one screen — **no API key**  
3. Table the asserts (command · pass · fail)  
4. Non-goals + composition (beside frameworks, not instead)  
5. Loud falsifier — claim dies if examples don’t go red  

## Weekly field remix (public)

Every week I take one strong public pattern (Promptfoo / DeepEval / AgentEvals / ECT / Hamel-style judges) and ship a **thin Homi remix**: same house voice, CI-green, hire-signal labels. Series tag: `field-remix`.

## Links

- GitHub: [@homayoun-safarpour](https://github.com/homayoun-safarpour)  
- LinkedIn: [in/homayoun-safarpour](https://www.linkedin.com/in/homayoun-safarpour/)  
- ORCID: [0000-0002-3206-5357](https://orcid.org/0000-0002-3206-5357)

Python 3.10–3.12 CI. Claims backed by named tests. Quickstarts under ~30 minutes.
