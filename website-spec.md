# STL Trash Valet — Website Specification

A single-page lead-generation website targeting **property managers** of apartment
complexes across the St. Louis Metro Area (both Missouri and Illinois sides).

The three core value propositions, in order of importance:
1. **Extra revenue** without extra work
2. **Ease of implementation**
3. **Local support**

---

## 1. Brand & Design System

### Logo
- File: `assets/logo.png`
- Vintage stamp / badge style, circular, forest green + cream.
- Used as a 44px circular mark in nav and footer, and as a large floating badge in the hero.

### Color Tokens
```
--ink:        #14201a    /* primary text */
--ink-soft:   #3a4a40    /* secondary text */
--muted:      #6b7a70    /* tertiary / captions */
--hairline:   #d9d2bf    /* borders */
--hairline-2: #e8e1cd    /* softer borders */

--green:      #1d4a2e    /* primary brand */
--green-dark: #0f2e1c    /* hover / deeper */
--green-deep: #0a2114    /* darkest, used for headlines + dark sections */
--green-mid:  #2d6a44    /* mid accent */
--green-soft: #eaf0e9    /* tint background */

--paper:      #faf7ee    /* primary background */
--paper-2:    #f5efdf    /* alt section background */
--paper-3:    #ebe2cc    /* deepest cream */
--cream-ink:  #f6f0df    /* on-dark text */

--gold:       #b8893a    /* accent (Illinois on map, highlights) */
--gold-soft:  #e9d8a6    /* on-dark accent */
```

### Typography
- **Display / Serif:** DM Serif Display — headlines and stat numbers
- **UI / Sans:** Manrope (400, 500, 600, 700, 800) — body, navigation, buttons, forms
- **Script:** Allura — handwritten phrases inside headlines (e.g. "New revenue,",
  "pays for itself —", "predictable NOI.", "Service Area", "questions property
  managers", "let's run the numbers"). Mirrors the "Trash Valet" signature in the logo.

### Layout Tokens
- Max content width: `1240px`
- Section vertical padding: `104px` (top/bottom)
- Section horizontal padding: `clamp(20px, 4vw, 56px)`
- Hairline borders, generous whitespace, light shadow depth.
- "Eyebrow" labels: 12px uppercase 0.18em letter-spaced sans, in brand green,
  prefixed with a 28px hairline rule.

---

## 2. Page Structure (top to bottom)

1. Sticky navigation
2. Hero
3. Stats strip (dark green band)
4. Pillars — Why STL Trash Valet (Revenue / Easy / Local)
5. How It Works — 4 steps
6. Revenue section + interactive calculator (dark green band)
7. Service Area — SVG bi-state map + city list
8. Testimonial quote (paper background)
9. FAQ — 8 expandable questions
10. Contact — info + lead form (dark green band)
11. Footer

---

## 3. Section-by-Section Content

### 3.1 Navigation (sticky, top)

**Brand:**
- Logo + name: **STL Trash Valet**
- Tagline beneath name: **Est. 2025 — St. Louis**

**Links:** Service · Revenue · Service Area · FAQ

**CTA button (right):** **Get a Proposal** (cream paper background, dark green text, hairline border — matches the site palette rather than fighting it)

---

### 3.2 Hero

**Eyebrow:** Serving properties from O'Fallon, MO to O'Fallon, IL

**Headline (with italic + script accents):**
> Doorstep trash, *handled.*
> *New revenue,* zero new work.

**Lede paragraph:**
> We collect trash from your residents' doors five nights a week and walk it to your on-site dumpsters. You add a popular amenity, generate margin on every door, and never lift a bag.

**Primary CTA:** Get a Property Proposal → (scrolls to #contact)
**Secondary CTA:** (314) 723-2893 (tel link)

**Trust row (small text under CTAs):**
- **5 nights** a week pickup
- Owner-operated, local STL
- $1M liability insured

**Hero visual:** large circular logo badge with subtle float animation, plus a floating "4.9 ★ Resident satisfaction" tag card.

---

### 3.3 Stats Strip (dark green band)

Four stats:
- **5×** — Nights per week pickup
- **120+** — Doors per route, scalable
- **$0** — Cost or labor to property
- **2 wks** — From contract to launch

---

### 3.4 Pillars — Why STL Trash Valet

**Eyebrow:** Why property managers choose us

**Headline:** An amenity that *pays for itself —* and then some.

**Lede:** Three things you care about. Three things we get right. No add-on fees, no resident complaints, no Monday-morning surprises.

#### Pillar 01 — Revenue
**Title:** Extra revenue, every door.
**Body:** Charge residents a doorstep-pickup amenity fee — typically $20–$30 per unit per month — and keep a healthy margin. Predictable, recurring NOI lift without raising rent.

#### Pillar 02 — Easy
**Title:** Two weeks to launch.
**Body:** Sign, share resident details, get marketing materials. We onboard your team, distribute branded bins to each unit, and start collecting on day one. Your office doesn't field a single call.

#### Pillar 03 — Local
**Title:** Owned & answered in STL.
**Body:** We're based in St. Louis. When something needs handling, you talk to the same person every time — not a call center. Same-night response on after-hours issues, both Missouri and Illinois sides.

---

### 3.5 How It Works — 4 Steps

**Eyebrow:** How it works

**Headline:** From signed agreement to *first pickup* in two weeks.

**Lede:** A four-step rollout designed so your team does almost nothing. We handle the logistics, the residents, and the bags.

#### 01 — DISCOVERY
**Title:** 30-minute walk-through
**Body:** Tour the property, count doors, confirm dumpster locations and route. You get a custom proposal within 48 hours.

#### 02 — SETUP
**Title:** Branded bins delivered
**Body:** We drop a 13-gallon, lidded valet bin at every door with a welcome flyer explaining pickup nights and rules.

#### 03 — LAUNCH
**Title:** Five nights a week
**Body:** Sunday–Thursday between 8 PM and midnight, our team walks every floor, every door. Bags go to the on-site compactor or dumpster.

#### 04 — REPORTING
**Title:** Monthly snapshot
**Body:** Pickup counts, exception reports, and resident feedback delivered to your inbox. One point of contact, every month.

---

### 3.6 Revenue Section + Interactive Calculator (dark green band)

**Eyebrow:** The math is the easy part

**Headline:** Turn nightly trash into *predictable NOI.*

**Lede:** A doorstep valet program is the highest-ROI amenity you can add. No capital outlay, no staff to hire, no equipment to maintain. The revenue lift flows straight to NOI.

**Bullet list (with check icons):**
- No capital expense — we provide bins, labor, insurance.
- Bill residents directly on your existing ledger.
- Margin in the $8–$15 per unit per month range.
- Cleaner property, fewer hallway-trash complaints.

#### Calculator (paper card, right side)
**Title:** Estimate your annual lift

**Inputs (sliders):**
- **Number of units** — range 24 to 500, step 4, default 120
- **Margin per unit / month** — range $5 to $18, step $1, default $10

**Output:**
- Label: "Estimated annual revenue lift" + small line "Margin × Units × 12 months"
- Live formula: `units × margin × 12` → formatted as currency, suffix " /yr"
- Default display: **$14,400 /yr**

**Footnote:** Illustrative only. Actual margin depends on resident pricing, take-rate, and contract terms.

---

### 3.7 Service Area

**Eyebrow:** Service area

**Headline:** The whole STL Metro — *both sides* of the river.

**Lede:** Properties from West County to the Metro East. If your property is within the I-270/I-255 loop or close to it, we're already running a route nearby.

**Map (custom SVG):** Stylized two-state shape, Missouri rendered in soft green, Illinois in soft cream/gold, river curve between, city dots, and a "★ HQ · St. Louis" marker.

**Legend:** Missouri side · Illinois side · ★ HQ — St. Louis, MO

**Cities list (right column, headed "Cities we serve"):**

Missouri:
- St. Louis City
- Clayton
- University City
- Maplewood
- Kirkwood
- Webster Groves
- Chesterfield
- Creve Coeur
- Ballwin
- Florissant
- Hazelwood
- Arnold
- Fenton
- O'Fallon, MO
- St. Charles
- St. Peters

Illinois:
- Belleville, IL
- Fairview Heights, IL
- O'Fallon, IL
- Edwardsville, IL
- Collinsville, IL
- Columbia, IL
- Granite City, IL
- Swansea, IL

**Sub-lede above the list:** Selected service areas across the STL Metro. Don't see your property? We're almost certainly close — call us.

---

### 3.8 Testimonial Quote

Large serif blockquote, centered, paper background:

> Residents stopped leaving bags in the hallways the week we launched. Our front office got a quiet night back, and the program runs itself.

**Attribution:** Regional Property Manager · 240-unit community, West County

---

### 3.9 FAQ — 8 questions (accordion)

**Eyebrow:** FAQ

**Headline:** Questions *property managers* ask first.

**Lede:** Quick answers. If yours isn't here, the contact form goes straight to the owner.

---

**Q1: What does it cost the property?**
Nothing. Our model bills residents directly through your existing rent ledger as a mandatory amenity. The property keeps a margin per unit per month and we keep the rest. Zero capital expense, zero labor cost.

**Q2: Do I have to make residents use it?**
Mandatory programs perform best — they spread cost across all units and dramatically reduce hallway-trash issues. We can also structure as an opt-in or move-in amenity. We'll recommend the right structure during your discovery call.

**Q3: What nights and times do you pick up?**
Sunday through Thursday, between 8 PM and midnight. Residents are asked to set their bagged trash outside their door no earlier than 6 PM that evening. We can customize the schedule for properties with quiet-hours policies.

**Q4: Where does the trash actually go?**
Straight to your on-site dumpsters or compactor. We don't haul off-site — your existing waste hauler handles disposal as normal. We're an amenity service, not a hauling service.

**Q5: What about recycling and bulk items?**
Recycling pickup runs once a week on a day we'll set with you. Bulk items (boxes, furniture) are handled by appointment with a small added fee billed to the resident — never to the property.

**Q6: Are you insured? Bonded?**
Yes. $1M general liability, workers' comp, and commercial auto on every vehicle. On request, we'll add your property and ownership group as a named party on our policy — meaning you're directly covered by our insurance for any incident involving our crew, at no cost to you. Certificates of insurance are provided within 24 hours.

**Q7: How long is the contract?**
Standard agreements are 12 months with auto-renewal. There's a 60-day out clause if performance falls short of agreed service standards — so you're never locked in if we don't deliver.

**Q8: Do you cover the Illinois side of the Metro?**
Yes — Belleville, O'Fallon, Edwardsville, Fairview Heights, Collinsville, Columbia, Granite City, and surrounding communities. We're a true bi-state operator, not a Missouri-only outfit.

---

### 3.10 Contact Section (dark green band)

#### Left column

**Eyebrow:** Get a proposal

**Headline:** Let's run the *numbers* for your property.

**Lede:** Tell us a little about the community and we'll send a custom revenue estimate within one business day. No pressure, no boilerplate.

**Contact info list:**
- **Call us direct:** (314) 723-2893 (tel:3147232893)
- **Email sales:** sales@stltrashvalet.com (mailto)
- **Office hours:** Mon–Fri · 8a – 6p CT

#### Right column — Lead form (paper card)

**Title:** Request a property proposal
**Subtitle:** Takes about 60 seconds. Owner-reviewed within one business day.

**Fields (in order, * = required):**

| Field            | Type     | Required | Options / Notes |
|------------------|----------|----------|------------------|
| Your name        | text     | yes      | autocomplete=name |
| Role             | select   | no       | Property Manager / Regional Manager / Owner / Asset Manager / Maintenance Director / Other |
| Work email       | email    | yes      | regex-validated |
| Phone            | tel      | no       | placeholder "(314) 555-0123" |
| Property name    | text     | yes      | |
| Unit count       | select   | yes      | Under 50 / 50–100 / 100–200 / 200–350 / 350+ units |
| Anything we should know? | textarea | no | "Existing valet contract, timeline, special access notes, etc." |

**Submit button:** Send my proposal request →

**Legal line beneath button:** We'll never share your details. One follow-up email per request, max.

**Success state (replaces form on successful submit):**
> **Thanks — we've got it.**
> Your request is in. We'll review and send a tailored proposal within one business day. Need to talk sooner? Call **(314) 723-2893**.

---

### 3.11 Footer

**Brand column:**
> Doorstep trash collection for apartment communities across the St. Louis Metro Area. Owner-operated. Locally answered. Established 2025.

**Service column:**
- How it works
- Revenue model
- Service area
- FAQ

**Contact column:**
- (314) 723-2893
- sales@stltrashvalet.com
- Request a proposal

**Coverage column:**
- St. Louis County
- St. Charles County
- Madison County, IL
- St. Clair County, IL

**Bottom row:**
- © 2025 STL Trash Valet, LLC. All rights reserved.
- Owner-operated · Licensed & insured · Serving STL bi-state

---

## 4. Interactions / JS Behavior

- **Sticky nav** — adds a hairline bottom border on scroll past 8px.
- **Reveal-on-scroll** — pillars and how-it-works steps fade up via IntersectionObserver on enter (threshold 0.12), one-shot.
- **FAQ accordion** — click toggles `.open`, animates `max-height` from 0 → `scrollHeight`. The "+" rotates 180° and inverts to green-on-paper. One item at a time is acceptable; current implementation allows multiple open.
- **Revenue calculator** — two `<input type="range">` controls update labels live, recalculate `units × margin × 12`, format as `$X,XXX /yr`.
- **Contact form validation:**
  - Required: name, email, property name, unit count.
  - Email validated with regex `^[^\s@]+@[^\s@]+\.[^\s@]+$`.
  - Errors show inline (red border + small red error text) on blur and on submit.
  - On valid submit: form switches to a success state (no real backend wired yet — see Next Steps).

---

## 5. Business Details (single source of truth)

- **Business Name:** STL Trash Valet
- **Phone:** 314-723-2893
- **Email:** sales@stltrashvalet.com
- **Domain:** www.stltrashvalet.com
- **Service area:** St. Louis Metro, Missouri and Illinois sides
- **Established:** 2025

---

## 6. Files in This Project

```
index.html         — the full single-page site
assets/logo.png    — circular vintage-stamp logo
website-spec.md    — this document
```

---

## 7. Suggested Next Steps (not yet built)

- Wire the contact form to a real backend (Formspree, HubSpot, Netlify Forms, or a Supabase edge function).
- Replace floating tags / map / testimonial with real photography:
  - Resident bag at door (lit, dusk).
  - Branded 13-gal valet bin closeup.
  - Crew on route (uniformed, friendly).
- Add `/privacy` and `/terms` pages.
- Add Open Graph meta tags + favicon variants (the favicon already references the logo).
- Add GA4 + a Meta Pixel for ad attribution.
- Real testimonials with named properties (with permission).
- Optional: a "case study" sub-page with one detailed property example.
