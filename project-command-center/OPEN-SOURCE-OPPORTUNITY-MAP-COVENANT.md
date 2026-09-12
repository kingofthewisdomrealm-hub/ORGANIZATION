# OPEN SOURCE OPPORTUNITY MAP — COVENANT

**Repo:** kingofthewisdomrealm-hub/COVENANT  
**Commit scanned:** 1533a055 (main)  
**Live:** https://covenant-builders-ten.vercel.app  
**Date:** 2026-09-12  
**Scout rule:** do not replace working custom code that is the product.

## What this repo actually is

Next.js 14 marketing site for Covenant Builders.

Already in place (do not rip out): Tailwind + custom brand UI; Zod + next-safe-action; Resend; Supabase anon key → `submit_website_lead` RPC; Cal.com embed with phone fallback; Vercel Analytics; next/og; custom storm quiz with Florida advertising-law copy; custom floor-plan sketcher; custom /play game; custom homeowner-programs explorer.

No Google Maps. No Mapbox. No auth. No CMS. No search engine.

## OPEN SOURCE OPPORTUNITY MAP

| Project Capability | Current Method | Open-Source Opportunity | Candidate | Benefit |
| --- | --- | --- | --- | --- |
| Lead capture | Custom forms → CRM RPC + Resend | Leave | Existing `lib/crm.ts` | Right shape. Do not put a CRM product on the public site. |
| CRM admin | Separate convenantbuilderscrm | Modify (other repo) | Atomic CRM | This site writes leads. Admin UI is the other app. |
| Storm event matching | 2 hand-entered events + ZIP table | Combine | NWS/SPC via IEM + keep quiz | Stops the table rotting. Legal copy stays ours. |
| Weather context | None | Use | Open-Meteo API | Recent wind/hail without a vendor. |
| Address → map | Plain text | Combine later | MapLibre + PMTiles | Pin the house. Not required to take a lead. |
| Booking | Hosted Cal.com | Leave | `@calcom/embed-react` | Working. Self-host is AGPL + ops. |
| Analytics | Vercel Analytics | Leave | Umami only if first-party is required | No conversion gain. |
| Rate limit | In-memory Map | Use small store | Upstash / Vercel KV | Serverless memory resets. |
| Floor-plan sketch | Custom SVG/canvas | Leave | — | Intentionally not CAD. |
| /play game | Custom React | Leave | — | Phaser is the wrong size. |
| Programs explorer | Custom 40k UI | Leave | — | Florida-specific rules. |
| Search / CMS / auth / email | Missing or Resend | Leave | — | Brochure site. |

## Decision

**COMBINE** storm data. **LEAVE** the site.

Ranked moves: (1) IEM/NWS feed into storm-check (2) shared rate limit (3) optional MapLibre (4) Atomic CRM on the CRM repo not this one.

Do not let a model invent storm events. Every displayed event needs a cited official source.
