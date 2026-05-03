# 3DAi VoiceLink — Website Overview
*Created: April 19, 2026 — Session 9*
*Last updated: April 19, 2026 — Session 9 (consolidation pass — trial variants added, Sitemap + Workflow linked)*
*Single source of truth for the website redesign. Read this first before any website work.*

---

## 1. What This Project Is

Redesign the customer-facing AI voice agent page for 3DAi VoiceLink.

| Field | Detail |
|---|---|
| **Brand** | 3DAi VoiceLink (subsidiary of TrezDev) |
| **Parent company** | TrezDev (trezdev.ai) |
| **Target page** | `https://trezdev.ai/ai-voice-agents` |
| **Standalone marketing domain** | AIPHONEAGENTS.BIZ |
| **Phone** | 866.390.3141 |
| **Owner** | Kevin (kevin@jigowattmedia.com) |
| **Out of scope** | TrezDev employee portal at `/auth/signin` (flagged for future fix — has no link back to main site) |

The `/ai-voice-agents` page is the primary revenue-driving surface. It's where inbound leads from ads, social, email, and outbound land. AIPHONEAGENTS.BIZ is the standalone marketing domain, but the canonical customer-facing experience we're improving lives on trezdev.ai.

---

## 2. Website Goals

1. **Hook the visitor in 3 seconds** with a clear value prop for AI voice agents.
2. **Introduce Grace** — the AI voice agent persona, front and center as the face of the brand.
3. **Walk through "How it Works"** visually, tied to the 3DAi System Infographic v3.
4. **Show the agent in action** via a live demo / click-to-call callback form (the strongest differentiator on the current site — keep it).
5. **Prove outcomes** with stats and industry-specific use cases.
6. **Convert** — Book a Demo as primary CTA, request-an-immediate-callback as secondary.
7. **Look clean, modern, confident** — not cluttered, not dev-themed, not generic SaaS.

---

## 3. Target Audience

Small and service-business owners who are stretched thin and can't afford to miss a lead.

- **Who:** Plumbers, HVAC, roofers, landscapers, dentists, med spas, real estate agents, contractors, salon owners, legal, insurance, home services.
- **Their world:** On a job site all day, missing calls, losing leads to faster competitors, can't justify a full-time receptionist, juggling too many tools.
- **Their language:** Plain, practical, show-me-the-money. No AI buzzwords. They care about booked appointments and saved time.
- **What they want to feel on the site:** "This is the future — and I can actually have this." Understood first, sold to never.

---

## 4. The Offer

**What we sell:** An AI voice agent ("Grace") that answers every call 24/7, has a natural human-like conversation, qualifies the lead, books the appointment, and drops everything into the CRM — plus the full Rebolt CRM + follow-up engine behind it.

**Pricing tiers** (from current site, refined in sitemap):

| Plan | Price | Minutes |
|---|---|---|
| Starter | $300 / mo | 500 |
| Pro (most popular) | $500 / mo | 1,000 |
| Business | $1,000 / mo | 2,500 |
| Enterprise | $1,500 / mo | 5,000 |

**Trial variants** (from `reference/3DAi VoiceLink – Sales Offers & Promo Menu.pdf` — sales uses these three as levers; the public site leads with #1):

1. **7-Day Full-Access Trial** — public-facing headline: "Try Free for 1 Week — No Credit Card Required."
2. **30-Day Trial After Go-Live** — sales-driven, unlocked once onboarding is complete.
3. **Usage-Based Trial** — first 100 answered calls free; reserved for strategic / partner deals.

Baseline promise on the site: **"No contracts. Cancel anytime."**

**Commitment levers** (sales can offer; site hints at them in Pricing): annual 10–15% discount, waived onboarding on annual, Founding-Customer Rate Lock (24 months).

**Primary CTA:** Book a Demo / Schedule a Call
**Secondary CTA:** Talk to Grace Right Now (live callback form)
**Tertiary:** Start Free Trial

---

## 5. Messaging Themes (Content Pillars)

These come directly from the brand voice doc and should thread through every section.

1. **Never miss a lead** — 62% of calls to small businesses go unanswered. Every missed call is missed revenue.
2. **AI that works for you** — Demystify AI. Friendly, not scary. 90%+ of callers can't tell it's AI.
3. **Small business, big advantage** — Level the playing field against bigger competitors.
4. **Replace the expense, keep the results** — A full-time receptionist is $35–50k/year. Grace is a fraction of that, no sick days, no turnover.
5. **The future is now** — Accessible, affordable AI. You don't need an IT department.

**Key stats to weave in:**
- 62% of calls to small businesses go unanswered
- 78% of customers buy from the first responder
- 24/7 coverage — no holidays, no sick days
- 90%+ of callers can't tell it's AI
- <5 second response time

**Brand voice in one line:** Warm but confident. No jargon. Short sentences. Active voice. Speaks to outcomes and feelings, not features and specs.

---

## 6. Design Direction

- **Lead with Grace** (the way Handshake leads with Julia) — personality before tech.
- **Dark theme** — navy base with cyan/blue accents, matching the infographic style.
- **Results-first** — like Rebolt: lead with outcomes ("+$380K revenue"), not features.
- **Clean and confident** — like Quo: lots of whitespace, one clear point per section, no clutter.
- **Live demo kept prominent** — the click-to-call callback is the strongest proof point we have.
- **Grace images** have transparent backgrounds and can be composited into any section (four outfits, see usage plan in `memory/projects/company-blueprint/website-sitemap.md`).

### Things to avoid
- TrezDev's dev-editor / file-tab aesthetic (doesn't match the service-business audience).
- Heavy gated forms on the homepage (Smith.ai approach is too much friction for our market).
- Jargon, hard selling, fear-mongering, corporate buzzwords.

---

## 7. Page Structure (Scroll Order)

Full detail in `memory/projects/company-blueprint/website-sitemap.md`. Summary:

1. **Hero** — Grace front and center. "Meet Grace. Your AI Phone Agent That Never Misses a Call." CTAs: Try Free + Watch Demo. Phone: 866.390.3141.
2. **The Problem** — 62% missed calls stat, pain points, animated counter.
3. **Meet Grace — How It Works (short version)** — 3-step visual: Customer Calls → Grace Answers & Books → You See Everything in CRM.
4. **Live Demo** — "Talk to Grace Right Now" callback form (keep from current site, refresh styling).
5. **Features — What Grace Can Do** — Feature cards: 24/7, natural conversations, qualifies leads, books appointments, confirmations, call recording + transcript, CRM integration, multilingual.
6. **The Complete System** — The 11-step customer lifecycle infographic (or interactive HTML version). Link out to full "How It Works" page.
7. **Industries We Serve** — Grid: home services, HVAC, plumbing, roofing, landscaping, legal, medical, insurance, real estate, etc. One-liner per industry.
8. **Results / Social Proof** — Stats bar (62%, 78%, 24/7, 90%+, <5 sec). Testimonial slots (placeholder until collected).
9. **Pricing** — 4 tiers + free trial offer.
10. **FAQ** — 8–12 questions (Handshake format).
11. **Final CTA** — Grace image again. "Ready to never miss another call?" Primary + secondary CTAs + phone.
12. **Footer** — Nav, phone, website, social, legal.

### Navigation
Home · How It Works · Solutions · Pricing · About · Contact / Demo

---

## 8. Important Pages / Surfaces

| Page | Purpose | Status |
|---|---|---|
| **Home (`/ai-voice-agents`)** | The main landing page — everything above | Redesign in progress |
| **How It Works** | Full 11-step customer lifecycle (blueprint + infographic) | To build |
| **Solutions** | Industry and use-case breakouts | To build |
| **Pricing** | Tiers + free trial + FAQ | To build (can live on home too) |
| **About** | Company story, Grace intro, TrezDev relationship | To build |
| **Contact / Demo** | Book a call, request demo, live callback | To build |

---

## 9. Key Assets On Hand

Everything lives in `reference/website-redesign/`:

- **`current-site/`** — Current TrezDev HTML template (what we're replacing).
- **`inspiration/`** — 5 reference site HTMLs: Rebolt, LeadTruffle, Handshake, Smith.ai, Quo. Each analyzed in `website-sitemap.md`.
- **`site-images/`** — 4 Grace images (transparent backgrounds). Outfit/usage map in sitemap.
- **`3DAi_System_Infographic_v3.png`** — Latest infographic for "How it Works" / "Complete System" section.
- **`SCOPE.md`** — The scope confirmation.

### Related docs outside this folder
- `memory/projects/company-blueprint/complete-company-blueprint.md` — Full 11-step lifecycle, all copy/content building blocks.
- `memory/projects/company-blueprint/website-sitemap.md` — Detailed section-by-section structure plan + reference-site analysis.
- `memory/projects/company-blueprint/3DAi_Complete_Customer_Lifecycle.png` — The full-lifecycle infographic.
- `skills/write-content/references/brand-voice.md` — Brand voice, tone, approved language, what to avoid.

---

## 10. Reference Site Takeaways (Cheat Sheet)

| Site | Borrow | Avoid |
|---|---|---|
| **Handshake** | Named AI persona (Julia → Grace), industry-specific demos, simple pricing, clean FAQ | Overly minimal footer |
| **LeadTruffle** | Testimonial carousel, integration logos, "organize by problem solved" use cases | Mega-menu complexity |
| **Smith.ai** | Industry segmentation | Gated homepage forms — too much friction |
| **Rebolt** | Results-first hero ("+$380K revenue"), "One platform" framing, industry grid, mobile-app callout | Over-packed sections |
| **Quo** | Polished visual design, whitespace, video in hero, star ratings, "The Difference" positioning | Too many sections for our scope |
| **Current TrezDev site** | Live callback form, pricing transparency, ROI stats | Dev-editor theme, TrezDev branding, no Grace, no testimonials, no "How It Works" |

---

## 11. Website Workflow / Status

From `memory/MASTER-CHECKLIST.md`:

- [x] Reference sites saved (Rebolt, LeadTruffle, Handshake, Smith.ai, Quo)
- [x] Current site saved (TrezDev template)
- [x] Company Blueprint complete (11 steps, 4 sections, infographic)
- [x] Scope locked — target page is `trezdev.ai/ai-voice-agents`
- [x] Sitemap / page-structure plan drafted
- [ ] **Design new page** (use inspiration + blueprint as guide) ← next
- [ ] **Build new page** (HTML/CSS/JS)
- [ ] **Kevin approval** — review and iterate
- [ ] **Swap live** — replace current `/ai-voice-agents` page with new design
- [ ] **(Future, separate task)** Fix employee portal so it has a "Back to main site" link

---

## 12. Non-Negotiables (Don't Break These)

- Phone number is **866.390.3141** — always. Never 566. Dot separator: `AIPHONEAGENTS.BIZ · 866.390.3141`.
- Grace is the face — every major section should either show her or reference her by name.
- Every section ends with a path to action (demo, callback, trial, pricing).
- No jargon. If a plumber can't understand a line, rewrite it.
- Mobile-first — this audience reads on phones between jobs.
- Preserve the live callback form from the current site — it's our single strongest proof of concept.

---

## 13. Open Questions (Confirm with Kevin Before Building)

1. **Domain / hosting** — Does the new page replace `trezdev.ai/ai-voice-agents` in place, or is AIPHONEAGENTS.BIZ going to become the canonical URL? Current scope says in-place on trezdev.ai.
2. **Pricing presentation** — Lead with 4 tiers, or simplify to a single "most businesses pick Pro" tier with the others on a pricing page? (Handshake went single-tier and it reads cleaner.)
3. **Testimonials** — Do we have any real ones ready to use, or do we launch with stats only and add quotes as they come in?
4. **Integrations logos** — Do we have confirmed integration partners to show (Jobber, Housecall Pro, ServiceTitan, etc.), or is that a phase-2 section?
5. **Free trial mechanics** — How does "Try Free for 1 Week — No Credit Card" actually work operationally? That copy is in the sitemap but the workflow behind it isn't locked.

---

## Quick Links
- Scope → `reference/website-redesign/SCOPE.md`
- **Sitemap (canonical) → `reference/website-redesign/Website-Sitemap.md`**
- **Workflow / build process → `reference/website-redesign/Website-Workflow.md`**
- Content source → `memory/projects/company-blueprint/complete-company-blueprint.md`
- Brand voice → `skills/write-content/references/brand-voice.md`
- Competitive pricing reference → `reference/Essential-Level Plans.pdf`
- Trial & promo variants → `reference/3DAi VoiceLink – Sales Offers & Promo Menu.pdf`
- Master checklist → `memory/MASTER-CHECKLIST.md`
