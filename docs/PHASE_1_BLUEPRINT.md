# Being of Earth (George Chountalos) — Phase 1 Blueprint

**Status:** Phase 1 Scaffolding & Wireframe (Framed in `src/index.html` & `src/style.css`)  
**Target Launch:** Before January 2027 (Ashley's Cutoff)  
**Hosting & Stack:** Cloudflare Pages (Static Edge, $0/mo)  
**Target Domain:** `www.beingofearth.com` (Root/WWW on Cloudflare; `go.beingofearth.com` remains on GoHighLevel)  
**Lead & Sales Engine:** GoHighLevel (Course, Member Portal, Billing, CRM)  
**Support Email:** `info@beingofearth.com`  
**Direct Support / WhatsApp:** `+52 999-551-8626`

---

## 1. Funnel & Architecture Overview
```
[ Word-of-Mouth / Past Clients / Organic Video / Future Traffic ]
                     │
                     ▼
  www.beingofearth.com (Cloudflare Pages Static Front Door)
  • Fast, earthy, authoritative aesthetic (JourneyImmersion + ZachBushMD vibe)
  • Video hero with George moving in nature
  • Clear educational hook: "Think like a health coach — become your own doctor"
  • Core focus: Kinesiology, Awareness, Four Pillars of Health
                     │
    ┌────────────────┼──────────────────────────────┐
    ▼                ▼                              ▼
[ PRIMARY CTA ]  [ SECONDARY LEAD CAPTURE ]   [ DIRECT CHAT / SUPPORT ]
14-Day Trial     Free 12-Page Workout Guide   WhatsApp: +52 999-551-8626
$45/mo           Email lead magnet capture    Email: info@beingofearth.com
    │                │                              │
    ▼                ▼                              ▼
go.beingofearth.com  GHL 5-Day Nurture Sequence   Direct personal conversion
(GHL Checkout)       → Converts to Trial          & Legacy $25/mo link
```

### Strategic Pricing Architecture:
* **Public Membership:** $45/mo with 14-day free trial. Cancel anytime with 1 click.
* **Alumni / Legacy Client Rate:** $25/mo locked in for life. Handled via unlisted GHL link / direct WhatsApp outreach to prevent public price cannibalization while seeding the community with high-engagement advocates.

---

## 2. Page Structure (Single High-Converting Long-Form Page)

### Section 1: Hero
- **Visual:** Clean full-width background video/loop of George doing functional mobility in nature (overlay with earthy dark tint for high text contrast).
- **Headline:** *Understand Your Body's Blueprint. Master Your Health.*
- **Subheadline:** A holistic, movement-first membership designed to teach you how to think like a health coach—so you can end chronic pain and restore vitality without generic workout burnout.
- **Primary CTA:** `[Start Your 14-Day Free Trial]` → links directly to GHL checkout.
- **Secondary CTA:** `[Download Free Workout Blueprint]` → scrolls to lead capture section.
- **Sub-badge:** *"14 Days Free • Cancel Anytime • Built for Americans & Canadians"*

### Section 2: The Problem ("Why Conventional Fitness Keeps Breaking You")
- Highlight the pain points George identified:
  - Cookie-cutter bootcamps that leave 40+ adults injured.
  - Mindless fitness apps that spit out sets/reps without understanding *why* your body hurts.
  - Outsourcing health decisions to temporary quick fixes.

### Section 3: The Being of Earth Methodology (The 4 Pillars)
1. **Movement & Mobility:** Kinesiology-grounded alignment, tension balancing, antagonist muscle mechanics.
2. **Nutrition & Biology:** Fueling cellular recovery and reducing systemic inflammation.
3. **Emotional Resilience:** Nervous system regulation and stress load management.
4. **Restorative Recovery:** Sleep optimization, circadian rhythm, and soft tissue care.

### Section 4: Free Guide Lead Magnet ("Create the Perfect Workout")
- High-converting bridge capturing the 90%+ of cold visitors who won't commit to a paid trial on visit #1.
- Features George's 12-page guide graphic.
- Connects to GHL email nurture sequence.

### Section 5: What’s Included in the Membership (Journey Immersion Style)
- **Weekly Live Coaching & Q&A Calls with George**
- **The Complete Step-by-Step Educational Curriculum** (Four Pillars of Health Assessment is Step 1)
- **Guided Video Routines & Progressive Protocols**
- **Private Community of Like-Minded Practitioners**
- **Direct Access & Program Guidance**

### Section 6: Meet George Chountalos
- High-authority, approachable founder bio:
  - Decades of real-world coaching experience across personal training and kinesiology.
  - Shifted away from typical gym superficiality to deep, lasting physiological transformation.
  - Authentic, grounded teaching style.

### Section 7: Client Transformations / Social Proof
- Real testimonials & quote cards with avatars (Art Allard, Lisa Marcoux, Layla, etc.) who restored mobility and eliminated chronic pain.

### Section 8: Final Call to Action, Pricing & Legacy Offer
- Bold headline: *Take the Reins of Your Health Today.*
- `[Start Your 14-Day Free Trial]` button ($45/mo after trial).
- **Alumni Special Callout:** "Former 1-on-1 Client of George? Get locked-in Legacy Access for just $25/mo via WhatsApp or email."

### Section 9: FAQ Accordion
- Native `<details>` tags addressing injury safety, daily time commitment, free trial cancellation, and Legacy $25 rate redemption.

### Section 10: Footer & Floating WhatsApp Widget
- Clean links, copyright, and direct links to:
  - `info@beingofearth.com`
  - WhatsApp: `+52 999-551-8626`
- Persistent floating WhatsApp quick-chat widget for direct conversions.
