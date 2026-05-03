# Website Redesign — Scope

*Last updated: April 19, 2026 — Session 9*

## Corporate Structure

- **TrezDev** is the parent company (domain: `trezdev.ai`).
- **3DAi VoiceLink** is a subsidiary brand within the TrezDev family, focused on AI voice agents.

## Target Page

**URL:** `https://trezdev.ai/ai-voice-agents`

This is the customer-facing page that potential customers land on when exploring the 3DAi VoiceLink AI voice agent product. **This is the page we are redesigning.**

The existing TrezDev site mixes a customer experience (the `/ai-voice-agents` marketing page) with a team/employee portal (`/auth/signin`) that is reached via a small "Employee Area" link in the footer. The redesign targets ONLY the customer-facing page. The employee portal is out of scope for this project.

## Why This Page

- It's the primary revenue-driving surface for the 3DAi VoiceLink offering.
- It's where inbound leads (from ads, social, email, outbound) will be sent.
- AIPHONEAGENTS.BIZ is the standalone marketing domain but the canonical customer-facing experience we're improving lives at `trezdev.ai/ai-voice-agents`.

## What the Page Needs to Do

Based on the Company Blueprint (see `memory/projects/company-blueprint/`) and the inspiration sites (Rebolt, LeadTruffle, Handshake, Smith.ai, Quo):

1. Hook the visitor in 3 seconds — clear value prop for AI voice agents.
2. Walk through "How it Works" visually (tie to the 3DAi System Infographic v3).
3. Show the voice agents in action (live demo / click-to-call).
4. Industries served and use cases.
5. Pricing tiers — Starter, Pro, Enterprise.
6. Primary CTA: Book a Demo / Schedule a Call.
7. Secondary CTA: Request an immediate callback from an AI agent.

## Known Issue on Current Site (Future Fix — Out of Scope Here)

The footer "Employee Area" link sends visitors to `/auth/signin` with no link back to the main site. A curious customer who clicks it gets stranded. Note this for the separate employee-portal task.

## Assets On Hand

- `current-site/` — current TrezDev HTML template for reference
- `inspiration/` — 5 reference site HTMLs (Rebolt, LeadTruffle, Handshake, Smith.ai, Quo)
- `3DAi_System_Infographic_v3.png` — latest infographic for the "How it Works" section
- `site-images/` — 4 Grace images (transparent backgrounds), usage map in `Website-Sitemap.md`
- `Website-Overview.md` — single source of truth for the redesign
- `Website-Sitemap.md` — page-by-page structure + reference-site analysis
- `Website-Workflow.md` — how we go from plan → design → build → launch

## Out of Scope (explicit)

- TrezDev employee portal at `/auth/signin` (has no "back to main site" link — noted for future fix)
- TrezDev parent-company marketing pages unrelated to `/ai-voice-agents`
- Sales-internal lead CRM (`Lead Data Collection & Management.pdf`) — that's ops, not website
- Social media campaign (`3DAi_Voicelink_Marketing_Campaign.docx`) — separate project
- Email/SMS sequence content — separate project
