# 3DAi VoiceLink — Website Workflow
*Last updated: April 19, 2026 — Session 9*
*How we go from plan → design → build → launch. One file for the process, so nothing slips between sessions.*

---

## 1. Current Status

| Phase | Status | Owner |
|---|---|---|
| Plan — scope, sitemap, content blueprint | ✅ Complete | Kevin + Claude |
| Reference + current site saved | ✅ Complete | Kevin |
| Infographic v3 built | ✅ Complete | Kevin + Claude |
| Grace images prepped (4 outfits, transparent) | ✅ Complete | Kevin |
| **Design mockup** | 🟡 Next | Kevin + Claude |
| Build (HTML/CSS/JS) | ⬜ After design approval | Claude |
| Kevin review + iterate | ⬜ | Kevin |
| Swap live at `trezdev.ai/ai-voice-agents` | ⬜ | Kevin |

---

## 2. Phases

### Phase 1 — Plan *(complete)*

Artifacts in this folder:
- `SCOPE.md` — what we're building and what's out of scope
- `Website-Overview.md` — single source of truth (audience, offer, messaging, design direction)
- `Website-Sitemap.md` — section-by-section structure + sub-pages
- `current-site/` — what we're replacing
- `inspiration/` — 5 reference sites
- `3DAi_System_Infographic_v3.png` — How It Works visual
- `site-images/` — Grace photography

### Phase 2 — Design *(next)*

Goal: a static visual mockup of the home page that Kevin can approve before we write code.

1. Pick the design tool. Options:
   - **HTML + Tailwind mockup** (single-file artifact in this folder) — fastest iteration, closest to production, no Figma round-trip.
   - **Figma** — better for pixel comps if Kevin wants design-first polish.
   - Default: **HTML + Tailwind**, unless Kevin calls for Figma.
2. Build the home page section-by-section in the order in `Website-Sitemap.md`.
3. Drop Grace images in per the usage map.
4. Apply dark theme (navy base, cyan/blue accents from infographic).
5. Use real copy from `Website-Overview.md` and `complete-company-blueprint.md` — no lorem ipsum.
6. Save iterations as `mockup-v1.html`, `mockup-v2.html`, etc. in this folder.
7. Kevin reviews → notes → next iteration. Loop until approved.

**Approval checkpoint:** Kevin signs off on the final mockup before any production build starts.

### Phase 3 — Build

Goal: production-ready HTML/CSS/JS that can be dropped into the existing trezdev.ai site at `/ai-voice-agents`.

1. Confirm the existing site's tech stack by inspecting `current-site/TrezDev - Modern Software Development.html` (framework, CSS approach, asset loader).
2. Match the build to that stack, or document why a rewrite is needed.
3. Production file structure (tentative):
   ```
   ai-voice-agents/
   ├── index.html
   ├── css/main.css
   ├── js/main.js
   ├── js/callback-form.js       ← keep working live-demo form
   ├── images/
   │   ├── grace-hero.png
   │   ├── grace-about.png
   │   ├── grace-cta.png
   │   ├── grace-faq.png
   │   └── system-infographic-v3.png
   └── README.md
   ```
4. Wire up:
   - Callback form (preserve existing backend).
   - Calendly / booking CTA.
   - Analytics (confirm existing tag with Kevin — GA4? Plausible?).
   - Phone number as clickable `tel:` link everywhere.
5. Pass the `Website-Sitemap.md` checklist before handoff.

### Phase 4 — Review & Iterate

1. Claude hosts the build locally (or writes to `reference/website-redesign/build/`) and shares a preview link or file.
2. Kevin reviews on desktop **and phone** (the audience is mobile-first).
3. Track revisions in a short `revisions-log.md` created at this phase.
4. Loop until Kevin says ship.

### Phase 5 — Launch

1. Final content + legal review — privacy policy, terms, accurate claims.
2. QA checklist (see §5 below).
3. Kevin (or dev contact at TrezDev) deploys to `trezdev.ai/ai-voice-agents`, replacing the current page.
4. Verify live on desktop + mobile + in several browsers.
5. Update `memory/MASTER-CHECKLIST.md` — mark "Swap live" complete, move project to Completed section.

### Phase 6 — Post-launch *(separate task, noted)*

- Fix employee-portal stranding: add a "Back to main site" link on `/auth/signin`.
- Add testimonial quotes as they come in.
- Add integration partner logos (Jobber, Housecall Pro, ServiceTitan, etc.) once confirmed.
- Decide: does AIPHONEAGENTS.BIZ become a 301 → `trezdev.ai/ai-voice-agents`, or stay as a secondary landing?

---

## 3. Roles & Handoffs

| Role | Owner | Notes |
|---|---|---|
| Product / offer decisions | Kevin | Pricing, trial structure, industries to list |
| Content / copy | Kevin + Claude | Copy pulled from blueprint + brand-voice doc, Claude drafts, Kevin edits |
| Design mockup | Claude | HTML/Tailwind in this folder, Kevin approves |
| Build | Claude | Production HTML/CSS/JS |
| Deploy | Kevin / TrezDev dev contact | Final push to trezdev.ai |
| QA | Kevin | Desktop + mobile verification |

---

## 4. Open Decisions (from Overview §13)

Claude will ask Kevin to resolve these **before Phase 2 (design)** so we don't rebuild mid-stream:

1. **Domain / hosting** — in-place replacement at `trezdev.ai/ai-voice-agents`? (Current scope says yes.)
2. **Pricing presentation** — lead with all 4 tiers, or single "Pro" headline with the rest on a pricing page?
3. **Testimonials** — launch with real quotes or stats-only until collected?
4. **Integration logos** — do we have confirmed partners to show on launch?
5. **Free trial mechanics** — how does "Try Free for 1 Week" work operationally? (Menu lists 3 trial variants — which one is the public-facing default?)
6. **Analytics stack** — GA4, Plausible, something else? Need to confirm what's on trezdev.ai today.

---

## 5. Pre-Launch QA Checklist

Copy into a new file when we get close.

**Content**
- [ ] Phone number is `866.390.3141` everywhere (never 566). Always dot-separated.
- [ ] Website shown as `AIPHONEAGENTS.BIZ · 866.390.3141` in footer/contact.
- [ ] "A TrezDev company" credit in footer.
- [ ] Grace named in every major section.
- [ ] No jargon — a plumber can understand every line.
- [ ] All CTAs go somewhere (no dead buttons).

**Functional**
- [ ] Live callback form works end-to-end (Grace actually calls back).
- [ ] Book-a-Demo CTA opens real calendar.
- [ ] All `tel:` links dial on mobile.
- [ ] Free-trial flow is connected (or routes to sales).
- [ ] Form submissions log to CRM.

**Design**
- [ ] Looks right on iPhone (smallest common width ~375px) — mobile-first.
- [ ] Looks right on 1440 and 1920 desktop widths.
- [ ] Grace images load with transparent backgrounds (no white halos).
- [ ] Infographic is readable on mobile (swap to stacked version if needed).
- [ ] Dark theme is consistent — no stray light-theme sections.

**Performance**
- [ ] Images compressed (Grace PNGs, infographic) — LCP under 2.5s.
- [ ] No console errors.
- [ ] Lighthouse Performance > 85, Accessibility > 90, SEO > 90.

**SEO**
- [ ] Title: "AI Voice Agents for Small Businesses | 3DAi VoiceLink"
- [ ] Meta description under 160 chars, includes "AI voice agent" and "24/7 answering."
- [ ] Open Graph image + title + description set.
- [ ] H1 is the hero headline; one H1 per page.
- [ ] `/ai-voice-agents` has a canonical URL.

**Legal / Trust**
- [ ] Privacy Policy linked.
- [ ] Terms linked.
- [ ] No unsubstantiated claims (stats sourced or hedged).
- [ ] Cookie banner if TrezDev uses one today.

---

## 6. File Conventions (inside `reference/website-redesign/`)

- `SCOPE.md`, `Website-Overview.md`, `Website-Sitemap.md`, `Website-Workflow.md` — core docs, never delete.
- `current-site/` — freeze, don't edit.
- `inspiration/` — freeze, don't edit.
- `site-images/` — master Grace assets.
- `mockup-vN.html` — design iterations (in this folder, numbered).
- `build/` — production code (create at Phase 3).
- `revisions-log.md` — create at Phase 4.

When a file becomes an old draft, move it to `archive/previews/` (per folder rules in CLAUDE.md) rather than deleting.

---

## 7. Session Protocol for Website Work

At the **start** of any website session:
1. Read `CLAUDE.md` (root).
2. Read `Website-Overview.md`, `Website-Sitemap.md`, `Website-Workflow.md` in this folder.
3. Check current phase in §1 above. Confirm with Kevin before moving phases.

At the **end** of any website session:
1. Update §1 status table if anything shifted.
2. Update "Last updated" header.
3. Ask Kevin if any Overview/Sitemap/Scope edits are needed.
4. If revisions were made, log them in `revisions-log.md` (if in Phase 4+).
