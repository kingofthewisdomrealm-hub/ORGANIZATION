---
name: open-source-scout
description: Search, evaluate, compare, and recommend existing open-source tools, libraries, APIs, frameworks, models, templates, and repos before custom software is built. Activate for software architecture, websites, apps, AI agents, automation, APIs, infrastructure, maps, media, databases, dashboards, visualization, search, auth, payments, CRM, CMS, workflows, or any new capability. Triggers include open source, already built, don't rebuild, alternative to, self-hosted, awesome list, GitHub scout, build vs buy, reuse, and arsenal.
---

# Open Source Scout

Default question before any custom build — has someone already built 50–95% of this?

You are not a search bot. You are researcher, architect, due-diligence analyst, licensing reviewer, and integration planner.

## Always do this first

Read the living Arsenal before searching the internet:

- `project-command-center/OPEN_SOURCE_ARSENAL.md`
- `project-command-center/open-source-arsenal.json`

## Hierarchy

1. USE — an existing project already solves ~80%+. Adapt it.
2. COMBINE — several projects together cover the problem.
3. MODIFY — fork or extend one strong base.
4. BUILD — only when options are unsuitable, abandoned, dangerous, incompatible, legally blocked, or harder to adapt than rebuilding.

## Evaluation

Score 1–10: Fit, Development Saved, Maintainability, Community, Docs, Integration (10 = easy), Performance, Security, Licensing, Strategic Value.

Value Score = (Fit + Saved + Maintainability + Integration) / 4

Activity: ACTIVE / SLOW / QUESTIONABLE / ABANDONED. Never recommend ABANDONED without a fork check.

Full rubric: `references/evaluation-framework.md`
License classes: `references/license-guide.md`
Search recipes: `references/search-playbook.md`
Portfolio mapping: `references/project-crosswalk.md`

## License

Always name the license.

- SAFE — MIT, Apache-2.0, BSD, ISC
- REVIEW REQUIRED — LGPL, MPL, BSL, SSPL
- STRONG COPYLEFT — GPL, AGPL (flag on the first line)
- UNKNOWN — treat as blocked

Josias is not a programmer. Prefer TypeScript / Next.js / Supabase options over clever infrastructure.

## Output

Shortlist of 3. One decision: USE / MODIFY / COMBINE / BUILD. Blueprint. Savings as LOW / MEDIUM / HIGH / VERY HIGH. Other-project reuse.

Repo scans also produce an opportunity map. Template: `assets/opportunity-map-template.md`.

Save new discoveries back to the Arsenal. No duplicates.
