# Evaluation framework

Use this when scoring candidates. Keep SKILL.md short; this is the full rubric.

## Score 1–10 anchors

| Dimension | 1–3 | 4–6 | 7–8 | 9–10 |
| --- | --- | --- | --- | --- |
| Functional Fit | Adjacent domain, heavy rewrite | Covers the core noun, missing verbs | Covers 70–85% including main workflow | Purpose-built for this job |
| Development Saved | Wrapper only | Saves a feature | Saves a subsystem | Saves an entire product surface |
| Maintainability | Dead or single-maintainer radio silence | Slow, irregular releases | Regular commits, responsive issues | Predictable releases, multiple maintainers |
| Community | Almost no users | Niche, few examples | Real production users, answers exist | Large ecosystem, copies in the wild |
| Documentation | README only, stale | Partial docs | Docs + examples that match current API | Docs, tutorial, working demo |
| Integration Difficulty | New language + new infra + new mental model | New service to host | Same language, new library | Drop-in on our stack (TS/Next/Supabase) |
| Performance | Cannot handle likely load | Unknown, no evidence | Fine for our current scale | Proven above our scale |
| Security | Known critical CVEs, no process | Young, no audit, wide attack surface | Normal risk, updates ship | Auth/secrets handled well, history of patches |
| Licensing | Unknown, custom, Commons Clause | Strong copyleft on a hosted app | Weak copyleft / review-required | Permissive, no surprise |
| Strategic Value | Commodity we already have | Nice to have | Unlocks a capability we lack | Becomes reusable infrastructure across projects |

Value = (Fit + Saved + Maintainability + Integration Practicality) / 4

Activity: ACTIVE 30 days / SLOW 1–6 months / QUESTIONABLE 6–18 / ABANDONED 18+.

Savings language only: LOW / MEDIUM / HIGH / VERY HIGH. Never invent hours.
