# Elitagen Agent

Branded [Google Antigravity](https://antigravity.google) plugin for
**Elitagen** - the global multilingual ecosystem where medicine, science,
technology, and creative design converge.

**Expert Minds. Intelligent Innovation. - THINK. BUILD. EVOLVE.**

## What's inside

| Component | File | What it does |
| --- | --- | --- |
| Custom agent | `agents/elitagen-expert.md` | Multidisciplinary life-sciences innovation agent covering Elitagen's three verticals (data governance & AI enablement, scientific & creative production, health-tech program management). Selectable as primary via `/agents`, also delegatable as a subagent. |
| Always-on rule | `rules/AGENTS.md` | Brand voice (tone, multilingual discipline) plus compliance & ethics guardrails - HIPAA, GDPR, HITECH, CCPA/CPRA, ISO/IEC 27001, EU AI Act, NIST AI RMF, ISO/IEC 42001, OECD AI. No fabricated citations, no medical advice. |
| Skill | `skills/brand-kit/SKILL.md` | Official palette (hex), logo usage, typography guidance, tagline discipline, and voice checklist. Feed it to any deliverable that a client or partner will see. Invoke with `/brand-kit`. |
| Logo | `assets/logo.png` | 1:1 brand mark bundled for the Marketplace card. |

## Try it locally

```bash
# from the Antigravity CLI:
agy plugin validate --strict ./elitagen-agent   # 0 errors, 0 warnings
agy plugin install ./elitagen-agent
agy plugin list

# then in chat:
/agents                # select "elitagen-expert" as the primary agent
/brand-kit             # load the brand kit for a branded deliverable
```

In the Antigravity App the plugin appears under
**Customizations > Installed** with three starter-prompt chips.

## Scaffold status & next steps

This is a foundation to build on. Intended extension points:

- **Vertical subagents** - split `elitagen-expert` into focused read-only
  specialists (e.g. `data-governance-advisor`, `sci-creative-producer`,
  `healthtech-pmo`) that the primary agent delegates to.
- **Capability skills** - one skill per repeatable deliverable type
  (`concept-note`, `storyboard-brief`, `program-plan`, `ai-readiness-review`).
- **MCP server** (`mcp_config.json`) - wire live data sources
  (project tracker, literature search, brand asset CDN) once endpoints exist.
- **Lifecycle hooks** (`hooks.json`) - e.g. a `Stop` hook that appends the
  compliance reviewer note on clinical-adjacent outputs.

## Requirements

- Antigravity App or CLI (`agy`) for install/validate
- No API keys, no network access, no external services
