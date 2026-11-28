# Being of Earth — Master Design Standard & Quality Specification (v1.0)
**Client / Brand:** Being of Earth (George Chountalos)  
**Engineering Studio:** Cenote Softworks (Calvin Curtis Miller Jr. & Antigravity)  
**Applicability:** Static Website, GoHighLevel Portal (`go.beingofearth.com`), Interactive Diagnostic, PDF Workbooks, Email Templates, and Brand Collateral  
**Last Updated:** November 27, 2026  

---

## 1. The Core Brand Covenant & Aesthetic Identity

Being of Earth is an authoritative, kinesiology-grounded, transformative health and movement academy. It is **not** a generic Silicon Valley fitness SaaS, nor a sterile clinical medical portal, nor a noisy influencer workout app. 

### The Aesthetic Formula
* **Atmosphere:** Deep forest, warm organic limestone, hand-crafted gold accents, and warm linen paper surfaces. Think *Journey Immersion* meets *Zach Bush MD*—grounded, wise, sovereign, calm, and biological.
* **Tone:** Clinical authority without coldness; warm mentorship without gym hype.
* **Non-Negotiables:**
  * **Zero stark white plastic boxes** dropped onto dark backgrounds.
  * **Zero bloated, un-styled glyphs or giant solid checkmarks.**
  * **Zero badges floating on top of human faces.**
  * **Zero cramped padding**—breathing room and generous negative space are load-bearing brand assets.

---

## 2. The Two-Atmosphere Architecture (The "Light Room vs. Dark Room" Law)

Every screen, page, and module in Being of Earth belongs strictly to one of two atmospheres. **Crossing the boundary between them without an intentional full-section transition is an immediate QA failure.**

```
┌────────────────────────────────────────────────────────────────────────┐
│ ATMOSPHERE A: DARK FOREST (Moody, Elevated, Transformative)            │
│ Background: #0e1c15 (Forest Dark)                                      │
│ Surface / Cards: #14281f (Forest Surface) + 1px #c5a059 (Gold Sand)    │
│ Typography: Pure White (#ffffff) Serif Headers, Soft Sage (#a3baa0)    │
│ Used for: Hero, Pricing / Enrollment, Testimonial Quotes, Dark Footer  │
└────────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼ [Full Section Break Only]
┌────────────────────────────────────────────────────────────────────────┐
│ ATMOSPHERE B: WARM LINEN (Educational, Clear, Diagnostic)              │
│ Background: #faf8f5 (Linen Light) or #f3efe8 (Linen Card)              │
│ Surface / Cards: #ffffff (Pure White) + 1px #e3ded6 (Linen Border)     │
│ Typography: Deep Forest (#0e1c15) Headers, Muted Olive (#475e50) Body  │
│ Used for: Problem Breakdown, 4 Pillars, Diagnostic, Lead Magnet, FAQ   │
└────────────────────────────────────────────────────────────────────────┘
```

### The Cardinal Rule:
* **Never drop an Atmosphere B element inside an Atmosphere A container.**  
  *(Example: Slapping a white card with dark text into the dark pricing section creates a jarring "white sticker" look and hides external headers. Cards in Atmosphere A must use `#14281f` with a gold border).*
* **Never drop unstyled dark text into an Atmosphere A container.**  
  *(All text in Atmosphere A must be explicitly white, gold sand, or light sage).*

---

## 3. Sovereign Design Tokens & Color Standards

### Primary Color Palette
| Token Name | Hex Code | Role & Usage |
| :--- | :--- | :--- |
| `--color-forest-dark` | `#0e1c15` | Section background for Atmosphere A (Hero, Pricing, Footer). |
| `--color-forest-surface`| `#14281f` | Elevated card surface inside dark sections. |
| `--color-forest-border` | `#1f3d2f` | Subtle structural dividers in dark sections. |
| `--color-gold-sand` | `#c5a059` | Primary action accent, card borders, key prices, gold pills. |
| `--color-gold-hover` | `#b38e4a` | Hover states for primary gold buttons. |
| `--color-moss-green` | `#2d5a43` | Primary brand accent in light sections, secondary nav button. |
| `--color-linen-light` | `#faf8f5` | Page background for Atmosphere B (Educational sections). |
| `--color-linen-card` | `#f3efe8` | Elevated card surface in light sections. |
| `--color-linen-border` | `#e3ded6` | Subtle dividers in light sections. |
| `--color-text-dark` | `#0e1c15` | Body & header text in light sections (High contrast). |
| `--color-text-light` | `#ffffff` | Primary text in dark sections (Pure contrast). |
| `--color-text-muted` | `#a3baa0` | Subtitles, leads, and periods (`/month`) in dark sections. |

### Typography Scale
* **Serif Headings (Warm Authority):** `font-family: var(--font-serif)` (`'Playfair Display'`, Georgia, serif).
  * Section Headers: `clamp(2rem, 4vw, 3rem)` (32px–48px), `line-height: 1.15`, letter-spacing `-0.01em`.
  * Card Titles: `clamp(1.75rem, 3vw, 2.75rem)`.
* **Sans-Serif Body & UI (Clear Readability):** `font-family: var(--font-sans)` (`'Plus Jakarta Sans'`, system-ui, sans-serif).
  * Body: `1rem` (16px) to `1.125rem` (18px), `line-height: 1.6`.
  * Badges & Tags: `0.75rem` (12px), `font-weight: 700`, `letter-spacing: 0.12em–0.15em`, `text-transform: uppercase`.

---

## 4. Component Structural Blueprints

### A. The Monthly Membership / Pricing Card (Atmosphere A)
* **Container:** Center-aligned inside `.pricing-card-wrapper` (`max-width: 760px`).
* **Surface:** `background: var(--color-forest-surface)` (`#14281f`).
* **Perimeter:** `border: 1px solid var(--color-gold-sand)` (`#c5a059`).
* **Corner Radius:** `16px` (`--radius-card`).
* **Padding:**
  * **Desktop:** `48px` vertical, `32px` horizontal (`var(--space-12) var(--space-8)`).
  * **Mobile:** `32px` vertical, `20px` horizontal (`var(--space-8) var(--space-5)`). Never compress below 20px.
* **Internal Hierarchy (Top to Bottom):**
  1. **Title:** 2.75rem serif white (`#ffffff`).
  2. **Lead:** 1.15rem soft muted green (`#a3baa0`).
  3. **Price Block:** Gold `$` (2rem) + White `45` (5rem serif, tabular-nums) + `/ month` (1.25rem).
  4. **Trial Note:** Gold bold text (`Includes full 14-Day Free Access. Cancel anytime with 1 click.`).
  5. **Deliverables Divider:** `1px solid var(--color-forest-border)`, padding-top 24px.
  6. **Feature List:** Left-aligned 580px block with 20px gold outline stroked checkmarks (`stroke-width: 2.5`), light readable text.
  7. **CTA Button:** Large full-width gold pill (`.btn-primary.btn-block.btn-xl`), height 56px, bold dark text with hover arrow.
  8. **Trust Micro-Copy:** Soft white 13px line with lock icon.
  9. **Alumni Sub-Card:** Dashed gold box (`border: 1px dashed var(--color-gold-sand)`), WhatsApp green button + Email gold outline button. **Zero public mention of $25/mo or legacy discount pills (alumni rates are decoupled and handled 1-on-1 via private link to protect public price anchoring).**

### B. Founder Portrait & Experience Badges
* **Photo Frame:** Rounded corners (`16px`), warm subtle border, zero visual clutter directly over the image.
* **The No-Overlap Law:** **Experience badges, clinical credentials, and accolades must NEVER be positioned on top of George's face, neck, or chest.**
* **Placement:** Position badges below the photo as a dedicated metadata bar (`.about-experience-strip`) or adjacent in the copy column.

### C. Checkmarks and Feature Icons
* **Icon Spec:** 2px stroked Lucide-style SVG outlines (`viewBox="0 0 24 24"`, `fill="none"`, `stroke="currentColor"`, `stroke-width: 2.5`).
* **Colors:** Warm gold (`#c5a059`) in dark sections; Moss green (`#2d5a43`) in light sections.
* **Sizing:** Strict `20px x 20px` with `flex-shrink: 0`. Never allow unconstrained inline SVG rendering.

### D. Buttons & CTAs
* **Primary Gold Button (`.btn-primary`):**
  * `background: var(--color-gold-sand); color: var(--color-forest-dark); font-weight: 700; border-radius: 9999px;`
  * Hover: `background: #b38e4a; transform: translateY(-2px);`
* **Secondary Moss Button (`.btn-secondary-nav`):**
  * Light outline on desktop; **hidden on mobile (`<= 640px`)** to preserve a Single Focal Point.
* **Alumni WhatsApp Button (`.btn-alumni-wa`):**
  * Clean WhatsApp green (`#25d366`), dark text, pill shape.

---

## 5. Responsive Ceilings & Mobile Geometry

* **Single Focal Point in Mobile Header:** At screen widths `<= 640px`, only ONE action button may be displayed in the header (`Start Free Trial`). All secondary pill buttons must collapse to eliminate cluttered header wraps.
* **Above-the-Fold Mobile Height:** Mobile top banners, announcement bars, or breadcrumbs must never exceed **45px total height**, ensuring the hero headline remains immediately visible above the fold.
* **Touch Targets:** All interactive elements must maintain a minimum touch target of **44px x 44px**.
* **Horizontal Overflow:** `overflow-x: hidden` enforced at `html, body`. Zero horizontal jitter or side-scrolling allowed under any circumstance.

---

## 6. Standards for Extended Digital Products

When building or styling products beyond the static website for George, these exact specifications apply:

### 1. GoHighLevel Course Portal (`go.beingofearth.com`)
* Custom CSS injection must enforce `--color-forest-dark` (`#0e1c15`) sidebar navigation and warm linen card backgrounds for course modules.
* Video player frames must use `12px` border-radius and a subtle 1px border.
* Completion checkmarks must mirror the 2px outline gold standard.

### 2. PDF Workbooks & Lead Magnets ("Create the Perfect Workout", 4 Pillars Workbook)
* Cover Page: Atmosphere A (Forest Dark, gold foil serif title, George's centered photo with clean framing).
* Interior Body Pages: Atmosphere B (Warm linen background, crisp forest dark typography, 24px margins, clean callout boxes).
* Typography: Playfair Display for primary headers, Plus Jakarta Sans for instructions and checklists.

### 3. Email Templates (GoHighLevel Nurture Sequences)
* Clean single-column layout (max-width `600px`).
* Header: Forest dark strip with the Being of Earth emblem and gold accent line.
* Body: Clean warm white, 16px body copy, forest green subheadings.
* Primary Button: Gold sand rounded rectangle with bold dark forest text.

---

## 7. The 10-Point Pre-Deployment Field Inspection Checklist

Before **any** commit, release, or client handoff is shipped, the following 10 items must be verified:

| # | Inspection Checkpoint | Pass Criteria |
| :-: | :--- | :--- |
| **1** | **Atmosphere Integrity** | Zero white cards inside Atmosphere A (Dark Forest) sections; zero dark headers on dark backgrounds. |
| **2** | **Pricing Card Geometry** | Card uses `#14281f` with 1px gold border, 48px/32px padding, and contains all internal copy (no orphaned external headers). |
| **3** | **Alumni Sub-Card** | Dashed gold box is present at the base of pricing with working WhatsApp and Email links; zero public mention of $25/mo or legacy pills. |
| **4** | **Photo Clearance** | No floating badges, text, or pills overlap George's face or body. |
| **5** | **Icon Scalability** | All checkmarks are 20px stroked outline SVGs (`stroke-width: 2.5`), zero solid black/giant glyphs. |
| **6** | **Mobile Header Focal Point** | Mobile header (`<= 640px`) contains exactly ONE primary button; secondary button is hidden. |
| **7** | **Above-the-Fold Height** | Mobile hero content is immediately visible without scrolling past bloated banner bars. |
| **8** | **Missing CSS Audit** | `find_missing_css.py` returns **0 missing classes** across all HTML pages. |
| **9** | **Tag Balance & Lint** | HTML tag parser reports **0 unclosed tags** and valid DOM structure. |
| **10** | **Cache-Buster Sync** | Stylesheet link query (`style.css?v=X.X`) is incremented and synchronized across all pages. |

---

## 8. Enforcement & Ownership

This document is the permanent, sovereign blueprint for **Being of Earth**. Any future revision, new page scaffold, or digital product must be evaluated and approved against this standard before delivery.
