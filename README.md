# Elitagen Agent

Branded [Google Antigravity](https://antigravity.google) plugin for
**Elitagen** and the **Funvepsiarte | Elitagen** psychosocial ecosystem -
multidisciplinary health & life-sciences innovation.

**Expert Minds. Intelligent Innovation. - THINK. BUILD. EVOLVE.**

## What's inside

### Agents (`/agents`)

| Agent | Role |
| --- | --- |
| `elitagen-expert` | Primary orchestrator. Multidisciplinary life-sciences innovation across Elitagen's three verticals (data governance & AI enablement, scientific & creative production, health-tech PMO). Delegates psychosocial/expressive work to the specialists below. |
| `facilitador-expresivo` | Funvepsiarte expressive-therapy facilitator: step-by-step session/workshop/cycle design, audio-to-methodology, SMAPS field records. |
| `arquitecto-smaps` | Community psychosocial interventions on the IASC/MHPSS (SMAPS) pyramid, backed by the OIM manual summary. |
| `revisor-etico` | Ethical review and role-boundary clarity: facilitation/wellness vs. regulated clinical psychotherapy; consents, avisos eticos, referral protocols. |

### Skills (`/<skill-name>`)

| Skill | What it does |
| --- | --- |
| `facilitacion-expresiva` | Full Gem-ported protocol: welcome menu, one-question-at-a-time intake, input validation, 10-section session design, document generation. Reference: `references/registros-clinicos-campo.md`. |
| `smaps-intervencion` | SMAPS intervention architecture: profile routing, active-case rules, 6-block design, 12-point matrix. Reference: `references/resumen-smaps-oim.md` (OIM 2021 summary). |
| `limites-eticos` | Ethical-by-design review of texts/audios/materials; risk classification; ethical document drafting. |
| `expediente-intervencion` | **New composite pipeline**: design + ethics review + operational docs + monitoring indicators in one dossier - the end-to-end deliverable that chains the three skills above. |
| `brand-kit` | Official palette, logo usage, typography, tagline discipline, Funvepsiarte closing block, Spanish no-anglicism rule. |

### Rule

`rules/AGENTS.md` (always-on): brand voice, multilingual discipline, and
compliance & ethics guardrails - HIPAA, GDPR, HITECH, CCPA/CPRA,
ISO/IEC 27001, EU AI Act, NIST AI RMF, ISO/IEC 42001, OECD AI; no fabricated
citations; facilitation is never presented as clinical psychotherapy.

## Try it locally

```bash
agy plugin validate --strict ./elitagen-agent
agy plugin install ./elitagen-agent

# then in chat:
/agents                    # pick elitagen-expert, facilitador-expresivo, ...
/facilitacion-expresiva    # or jump straight into a skill
/expediente-intervencion   # full documented intervention pipeline
```

Or copy this folder to `~/.gemini/config/plugins/elitagen-agent/` and restart
the app.

## Roadmap

- **MCP server** (`mcp_config.json`) - literature search, project tracker,
  brand asset CDN.
- **Lifecycle hooks** (`hooks.json`) - e.g. a `Stop` hook that forces the
  ethics review (`limites-eticos`) before delivering therapy-adjacent
  documents.
- **More Gems** - remaining reference assistants can be ported as additional
  skills/subagents using the same pattern.

## Requirements

- Antigravity App or CLI (`agy`)
- No API keys, no network access, no external services
