---
name: focus-filter
description: Given current energy, time available, or a vague request, rank the active projects and propose the single best next move.
---

# Focus Filter Skill

## Goal
Protect Josias from decision fatigue. Always return one clear next action.

## Process
1. Load current-focus and decision rules.
2. Ask (if needed) how much time/energy is available right now.
3. Score only the active engines against that constraint.
4. Output: “The single highest-leverage move right now is X because Y. Next physical action: Z.”
