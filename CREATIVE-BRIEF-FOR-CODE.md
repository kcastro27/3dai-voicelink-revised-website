# 3DAi VoiceLink — Creative Brief for Code
*Single-file briefing. Code reads this BEFORE writing any HTML/CSS/JS.*
*Created: May 2, 2026 (Session 21). Living document — update when scope or decisions change.*

---

## 0. Why this file exists

This is the bridge between the **strategy/creative phase** (locked decisions, brand voice, target audience, what we're trying to feel) and the **build phase** (Code agent translating intent into HTML/CSS/JS). Anything Code needs to know to make the right call without re-asking Kevin lives here. If you're Code and you're about to ask Kevin a question, check here first — odds are it's already answered.

When something changes, edit this file. Don't fork it. One source of truth.

---

## 1. The one-line "why"

We are building a **standalone marketing site at `3daivoicelink.ai`** so 3DAi VoiceLink looks like a real, established, specialized AI voice-agent company — not a TrezDev subsidiary side project. The site exists to convert small/service-business owners into demos and free trials of Grace, our AI phone agent.

Perception is part of the sales strategy. The current TrezDev-hosted page (`trezdev.ai/ai-voice-agents`) undersells the brand. The new standalone site fixes that.

---

## 2. Project facts (don't get these wrong)

| Field | Value |
|---|---|
| Brand | 3DAi VoiceLink |
| Parent (footer credit only) | TrezDev |
| Target domain | `3daivoicelink.ai` (available, not yet secured) |
| Legacy URLs (transitioning) | `trezdev.ai/ai-voice-agents` and `AIPHONEAGENTS.BIZ` |
| Phone | **866.390.3141** — always. Never 566. |
| Phone display format | `AIPHONEAGENTS.BIZ · 866.390.3141` (dot separator) |
| AI persona name | **Grace** (flag: confirm no direct competitor uses "Grace" before locking everywhere) |
| Owner | Kevin (kevin@jigowattmedia.com) |

---

## 3. Creative goals (what the site must achieve)

In priority order. If a build decision creates a tradeoff, the higher item wins.

1. **Hook the visitor in 3 seconds.** Clear value prop. A plumber on a job site, scrolling on his phone between calls, gets it instantly.
2. **Make Grace the face.** Persona-forward, like Handshake leads with Julia. Grace appears prominently in hero, About, Final CTA — and is referenced by name throughout.
3. **Prove it works in real time.** The live callback form ("Talk to Grace Right Now") is the strongest differentiator — it must be prominent and frictionless. This is non-negotiable; it carries from the current site.
4. **Walk through "How it works" visually.** Tied to the 3DAi System Infographic v3 (`3DAi_System_Infographic_v3.png`). Three-step short version on home, full 11-step on the How It Works page.
5. **Show outcomes before features.** Lead each section with what the customer gets, not what the tech does. Rebolt-style "+$380K revenue" framing wherever real numbers exist; stats bar where they don't yet.
6. **Convert.** Primary CTA: **Book a Demo**. Secondary: **Talk to Grace Right Now** (live callback). Tertiary: **Start Free Trial**. Every section ends with a path to one of these.
7. **Look clean, modern, confident.** Not cluttered. Not dev-themed. Not generic SaaS. Establish that 3DAi VoiceLink is a serious specialist company.

---

## 4. Audience — who we are writing and designing for

**Who:** Small / service business owners. Plumbers, HVAC techs, roofers, landscapers, dentists, med spas, real estate agents, contractors, salon owners, legal, insurance, home services.

**Their world:** On a job site all day, missing calls, losing leads to faster competitors, can't justify a full-time receptionist, juggling too many tools, mobile-first, low patience for jargon.

**Their language:** Plain, practical, show-me-the-money. They care about booked appointments and saved time. No AI buzzwords.

**What they should feel on the site:** "This is the future — and I can actually have this." Understood first, sold to never.

**Implication for Code:**
- Mobile-first. This audience reads on phones between jobs. Design and build mobile, then scale up.
- Big tap targets. Thumb-friendly CTAs.
- Fast. No bloated frameworks if they hurt LCP.
- No jargon in microcopy. If a plumber can't parse a label, rewrite it.

---

## 5. Brand voice (one paragraph)

Warm but confident. No jargon. Short sentences. Active voice. Speaks to outcomes and feelings, not features and specs. Demystifies AI — friendly, not scary. Never fear-mongers, never hard-sells, never uses corporate buzzwords.

**Full reference:** `skills/write-content/references/brand-voice.md`

---

## 6. The offer (so Code knows what's actually being sold)

Grace is an AI voice agent that answers every call 24/7, has a natural human-like conversation, qualifies the lead, books the appointment, and drops everything into the CRM — plus the full Rebolt CRM + follow-up engine behind it.

**Pricing tiers:**

| Plan | Price | Minutes |
|---|---|---|
| Starter | $300/mo | 500 |
| **Pro** (most popular) | $500/mo | 1,000 |
| Business | $1,000/mo | 2,500 |
| Enterprise | $1,500/mo | 5,000 |

**Trial offers (public-facing):**
- Headline trial: **"Try Free for 1 Week — No Credit Card Required"** (the 7-Day Full-Access Trial)
- Other variants (30-day post-go-live, first-100-calls-free) are sales-driven — do NOT surface on the public homepage. They live in pricing footnotes or stay sales-only.

**Baseline promise:** "No contracts. Cancel anytime."

---

## 7. Messaging pillars + must-have stats

Thread these through every section.

**Pillars:**
1. Never miss a lead — 62% of small-business calls go unanswered. Every missed call = missed revenue.
2. AI that works for you — friendly, not scary. 90%+ of callers can't tell it's AI.
3. Small business, big advantage — level the playing field against bigger competitors.
4. Replace the expense, keep the results — full-time receptionist = $35–50k/yr. Grace is a fraction.
5. The future is now — accessible, affordable AI. No IT department required.

**Stats to weave in (the "stats bar" content):**
- 62% of calls to small businesses go unanswered
- 78% of customers buy from the first responder
- 24/7 coverage — no holidays, no sick days
- 90%+ of callers can't tell it's AI
- <5 second response time

---

## 8. Design direction (visual rules)

- **Lead with Grace.** Persona-forward, Handshake-style.
- **Dark theme.** Navy base with cyan/blue accents — matches the infographic palette. (Locked direction; specific tokens TBD during mockup pass.)
- **Outcomes-first layout.** Rebolt-style — outcome headline, supporting proof, then features.
- **Whitespace and clarity.** Quo-style — one clear point per section. No clutter, no over-packing.
- **Live demo prominent.** Callback form is the strongest proof point on the page.
- **Grace images are transparent PNGs.** Four outfits, mapped to sections (see §11).

**Things to actively avoid:**
- TrezDev's dev-editor / file-tab aesthetic. Wrong audience.
- Heavy gated forms on the homepage (Smith.ai-style). Too much friction.
- Jargon, hard selling, fear-mongering, corporate buzzwords.
- Mega-menus or overpacked nav.

---

## 9. Build approach (how Code should construct this)

This is locked from Session 10 (April 21, 2026). Read it carefully before opening an editor.

**LeadTruffle is the structural skeleton.** Use their section order, layout patterns, and component types as the starting scaffolding. **DO NOT copy-paste their HTML/CSS.** Rebuild structurally with our own content, our own styling, our own components.

**Enrichments allowed section-by-section.** Once the LeadTruffle-shaped skeleton is in place, Kevin reviews each section and pulls in upgrades from:
- **Handshake** — for persona-forward patterns (especially hero, industry-specific demos, FAQ)
- **Rebolt** — for outcomes-first headlines, industry grid, "+$ revenue" framing
- **Quo** — for whitespace, polish, video-in-hero, star ratings, "The Difference" positioning

This is the antidote to the Frankenstein problem: keep one skeleton, decide enrichments deliberately per section, log each decision in `Skeleton-Decisions.md` before writing code for that section.

**Verbiage is OURS.** We borrow structure, never copy. All copy in 3DAi VoiceLink brand voice. Never echo Handshake or LeadTruffle headlines.

**Wireframe → mockup → build.** Kevin explicitly wants visuals to react to, not written plans (see §13). Wireframe lives at `reference/website-redesign/wireframe-v1.html`. Lock each section in `Skeleton-Decisions.md` before the corresponding HTML/CSS gets written.

**Section-by-section rhythm.** Don't ship the whole site in one drop. Build a section, show Kevin, get a thumbs-up or a redirect, then move to the next. Hero is already locked (see §10).

---

## 10. What's already locked

### Strategy (locked April 21, 2026)
- Standalone site at `3daivoicelink.ai` (not a TrezDev subsidiary page)
- LeadTruffle skeleton + section-by-section enrichments
- Verbiage is ours, structure can be borrowed
- "Company" nav tab is the back-door routing point to TrezDev / employee portal — looks like a normal About to clients
- Parent-company credit is small footer-only ("A TrezDev Company")

### Section 1 — Hero (locked April 21, 2026)
- **Visual pattern:** Logo-forward, persona-forward, single primary CTA. Handshake-leaning.
- **Logo:** 3DAi VoiceLink at top of hero, prominent, no eyebrow text above it.
- **Grace:** transparent PNG, hero's visual centerpiece.
- **Hero CTA:** ONE primary CTA (exact wording TBD — "Book a Demo" or a Grace-specific variant).
- **Top-right nav actions:** Log In + a secondary CTA. The nav CTA wording must NOT echo the hero CTA so they don't compete.
- **Layout to decide during mockup:** centered vertical stack vs. Handshake-style split (Grace on one side, headline + CTA on the other). Try one in v1, swap if it doesn't feel right.
- **Copy guardrails:** don't echo Handshake/LeadTruffle headlines; no jargon a plumber can't parse; one clear value prop, not a paragraph.
- **Open flag:** confirm no direct competitor AI voice agent uses "Grace" before committing the name everywhere.

### Sections 2–12 — TBD
Sections 2 through Footer are sketched in `Website-Sitemap.md` but each must be locked individually in `Skeleton-Decisions.md` before Code writes that section. The current draft scroll order is:

2. The Problem (62% stat hero, pain points)
3. Meet Grace — How It Works (3-step short version)
4. Live Demo — "Talk to Grace Right Now" (callback form, **non-negotiable**)
5. Features — What Grace Can Do (organized by problem solved, not feature name)
6. The Complete System (infographic embed)
7. Industries We Serve (grid, one-liner per industry)
8. Results / Social Proof (stats bar; testimonials when available)
9. Pricing (4 tiers + trial)
10. FAQ (Handshake format, 8–12 Qs)
11. Final CTA (Grace image again, primary + secondary CTAs + phone)
12. Footer

### Nav (draft — revisit after sections lock)
Top nav L→R: Company · How It Works · Solutions · Pricing · Resources
Top-right: Log In · [secondary CTA]

---

## 11. Assets on hand (use these — don't generate new ones without asking)

All under `reference/website-redesign/`:

| Asset | Purpose | File |
|---|---|---|
| Current TrezDev page | Reference for what we're replacing | `current-site/TrezDev - Modern Software Development.html` |
| Inspiration: LeadTruffle | Structural skeleton — section order, layout patterns | `inspiration/LeadTruffle _ AI Speed-to-Lead for Home Service Pros.html` |
| Inspiration: Handshake | Persona-forward patterns, FAQ, industry demos | `inspiration/Handshake _ The AI Receptionist for Service Businesses.html` |
| Inspiration: Rebolt | Outcomes-first hero, industry grid | `inspiration/AI-Powered CRM & Marketing for Home Service Pros _ Rebolt.html` |
| Inspiration: Quo | Whitespace, polish, video-in-hero | `inspiration/Quo (formerly OpenPhone) _ Best Phone System for Startups & Small Businesses.html` |
| Inspiration: Smith.ai | Industry segmentation (only) | `inspiration/Smith.ai 24_7 AI Receptionists & Live Human Agents.html` |
| System infographic v3 | "How It Works" / "Complete System" section | `3DAi_System_Infographic_v3.png` |
| Wireframe v1 | The current section scaffolding to react to | `wireframe-v1.html` |
| Section-decision log | Living per-section lock log | `Skeleton-Decisions.md` |

**Grace images** — `reference/website-redesign/site-images/`, all transparent backgrounds:

| File | Outfit | Suggested section |
|---|---|---|
| `freepik_...085.jpg` | Beige/tan top | Hero — warm, welcoming |
| `freepik_...101.jpg` | Black sleeveless | About / Meet Grace |
| `freepik_...114.jpg` | Black blazer, white top | Final CTA, Pricing, Enterprise positioning |
| `freepik_...121.png` | Gray casual top | FAQ, approachable sections |

---

## 12. Reference-site cheat sheet (borrow / avoid)

| Site | Borrow | Avoid |
|---|---|---|
| **Handshake** | Named persona, industry demos, single-plan clarity, clean FAQ | Overly minimal footer |
| **LeadTruffle** | Structural skeleton, testimonial carousel, integration logos, problem-framed use cases | Mega-menu complexity |
| **Rebolt** | Outcomes-first hero, "one platform" framing, industry grid, mobile-app callout | Over-packed sections |
| **Quo** | Polished visuals, whitespace, video in hero, star ratings, "The Difference" positioning | Too many sections |
| **Smith.ai** | Industry segmentation only | Gated homepage forms (too much friction) |
| **Current TrezDev** | Live callback form, pricing transparency, ROI stats | Dev-editor aesthetic, TrezDev branding, no Grace, no testimonials, no "How It Works" |

---

## 13. How Kevin reviews work (so Code doesn't waste cycles)

Kevin prefers visual prototypes over written plans. Direct quote from Session 10: *"is there anyway to build this like super rough... we can go back and forth all day long but I need to see something to get a better idea of what is going to be created."*

**How to apply:**
- Default to "build a rough version first, then iterate section-by-section based on reaction."
- Don't pile up written questions and hypothetical outlines before putting something visible in his hands.
- Wireframes/mockups can be crude (gray boxes, placeholder text) early on — that's actually preferred because it keeps focus on structure, not polish.
- Lock each section's decisions in `Skeleton-Decisions.md` as you go, so context isn't lost between sessions.
- One section at a time. Hero → Section 2 → … → Footer. Don't ship the whole page in one drop.

---

## 14. Non-negotiables (don't break these)

- Phone is **866.390.3141** — every appearance. Never 566. Format: `AIPHONEAGENTS.BIZ · 866.390.3141`.
- Grace is the face — every major section either shows her or references her by name.
- Every section ends with a path to action (demo, callback, trial, pricing).
- No jargon. If a plumber can't understand a line, rewrite it.
- Mobile-first build order. Phones are the primary device.
- The live callback form survives — it is our single strongest proof of concept.
- LeadTruffle is the skeleton, not the source. Never copy their HTML/CSS or their copy.
- One CTA per section, primary. Don't compete CTAs against each other in the same viewport.

---

## 15. Open questions Kevin still has to answer

These are not Code's calls. If a section requires one of these to be resolved, stop and ask Kevin.

1. **Domain + hosting** for `3daivoicelink.ai`. Available, not yet secured.
2. **Fate of legacy surfaces** — what happens to `trezdev.ai/ai-voice-agents` and `AIPHONEAGENTS.BIZ` once the new site is live (redirect strategy).
3. **Founder headshot** — do we have one or is this a placeholder slot.
4. **Hero trial offer** — 7-day free vs. 100-calls free vs. demo-only as the headline.
5. **Pricing display on home** — 4 tiers vs. Pro-only with "see all plans" link.
6. **Testimonials** — do we have any real ones ready, or launch with stats only and add quotes as they come in.
7. **Integration logos** — confirmed partners to display (Jobber, Housecall Pro, ServiceTitan, etc.) or phase-2.
8. **Free trial mechanics** — operational workflow behind "Try Free for 1 Week — No Credit Card" is not yet locked.
9. **"Grace" name clearance** — quick competitor check before the name is committed everywhere.

---

## 16. File map for Code

When Code starts a build session, the relevant files are:

- **This file** (`CREATIVE-BRIEF-FOR-CODE.md`) — read first.
- `Skeleton-Decisions.md` — per-section locked decisions. Read before touching any section.
- `Website-Overview.md` — longer-form goals, audience, design direction (reference).
- `Website-Sitemap.md` — full scroll order draft + sub-page outlines (reference).
- `wireframe-v1.html` — current visual scaffolding to react against.
- `inspiration/*.html` — the five reference sites. Open the relevant one when working on the matching section.
- `current-site/TrezDev*.html` — what we're replacing. Lift the live callback form pattern.
- `site-images/` — Grace, transparent PNGs, four outfits.
- `3DAi_System_Infographic_v3.png` — for the "Complete System" section.
- `../../skills/write-content/references/brand-voice.md` — voice rules.
- `../../memory/projects/company-blueprint/complete-company-blueprint.md` — full 11-step lifecycle copy source.

---

## 17. Workflow — plan → design → build → launch

From `Website-Workflow.md`. Status as of May 2, 2026:

- [x] Reference sites saved (Rebolt, LeadTruffle, Handshake, Smith.ai, Quo)
- [x] Current site saved (TrezDev template)
- [x] Company Blueprint complete (11 steps, 4 sections, infographic)
- [x] Scope locked — standalone site at `3daivoicelink.ai`
- [x] Sitemap / page-structure plan drafted
- [x] Wireframe v1 built
- [x] Hero section (Section 1) locked
- [ ] **Lock Sections 2–12 one at a time** ← current phase (Kevin reviews + locks each)
- [ ] **Build the page** (HTML/CSS/JS) section-by-section as each section locks
- [ ] **Kevin approval** per section
- [ ] **Domain secured + hosting set up**
- [ ] **Swap live** — point `3daivoicelink.ai` at the new build
- [ ] **(Future)** Plan redirect strategy for `trezdev.ai/ai-voice-agents` and `AIPHONEAGENTS.BIZ`

---

*If anything in this brief is wrong, outdated, or missing — fix it here. This file is the source of truth for Code on the website project.*
