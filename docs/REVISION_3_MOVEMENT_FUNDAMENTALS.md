# Being of Earth — Revision 3: Movement Fundamentals & Holistic Intake Edition

**Release Date:** November 27, 2026  
**Status:** Live Staging Prototype on GitHub Pages  
**Live URL:** [`fundamentals.html`](https://cmiller1466-ship-it.github.io/Being_Of_Earth_George/fundamentals.html)  

---

## 1. Overview of Revision 3

Following George's overnight feedback and workbook expansion, this edition introduces two major strategic upgrades to the Being of Earth ecosystem:

1. **Evolution of the Free Lead Magnet:**
   * Replaced the introductory PDF (*"Create the Perfect Workout"*) with George's newly authored **40-page interactive digital workbook**:  
     **`Movement Fundamentals — Movement as Expression: A 5-Phase Strategy for Lifelong Participation`**
   * Features George's custom aerial drone cover artwork (`assets/images/movement-fundamentals-cover.jpg`).
   * Explicitly showcases the **5 Movement Phases**:
     - **01 Mobility:** Active joint synovial fluid circulation & spinal decompression
     - **02 Self-Massage:** Targeted trigger point release with lacrosse ball or foam roller (60s holds)
     - **03 Corrective Stretching:** Active elongation with 5–10 second contract-relax holds
     - **04 Resistance Training:** 7 Primal movement patterns capped at 30–40 min to prevent cortisol spikes
     - **05 Core Conditioning:** Restoring the neglected Transverse Abdominus (TVA) through diaphragmatic breathing
   * Incorporates interactive workbook elements: pre- and post-movement check-ins, the 7-day movement experiment, and lifelong participation reflection sheets.

2. **Re-Engineered 60-Second Holistic Health Diagnostic:**
   * Directly incorporates George's requested categorization of root health friction:
     - **[1] Physical Joints, Spine & Muscle Discomfort:** Chronic lumbar/neck stiffness, joint sensitivity, movement limitations.
     - **[2] Systemic, Cardiovascular & Metabolic Vitality:** Blood pressure, metabolic stamina, blood sugar stability, chronic systemic inflammation.
     - **[3] Digestive Health & Gut Vitality:** Sluggish digestion, bloating, food sensitivities, nutrient malabsorption, gut-brain connection.
     - **[4] Mental, Stress & Emotional Health:** Daily anxiety, mental fatigue, burnout, high nervous system stress, emotional overwhelm.
     - **[5] Daily Energy, Lethargy & Morning Fatigue:** Chronic morning fatigue, 3 PM energy crashes, poor sleep recovery.
   * **Legal & Regulatory Safeguard:** Includes an explicit FTC/medical compliance disclosure protecting George:
     > *"Being of Earth provides holistic health and movement education. This self-assessment is an educational reflection tool, not a medical diagnosis or treatment plan for chronic clinical conditions (such as cardiovascular disease, hypertension, or clinical depression). Always consult your qualified healthcare practitioner."*
   * Maps each respondent's friction point to their foundational root in the Four Pillars and provides a customized 5-phase starting roadmap + 1-click invitation into the 14-day free trial.

---

## 2. Multi-Version Staging Architecture

All three versions of the Being of Earth front door remain fully intact, interactive, and linked via the top evaluation toggle banner:

| Version | File | Purpose | Live Preview |
| :--- | :--- | :--- | :--- |
| **Revision 3** | `fundamentals.html` | **Movement Fundamentals & Holistic Intake Edition** (Latest founder vision, 40-page workbook, pain-point diagnostic) | [Open Revision 3](https://cmiller1466-ship-it.github.io/Being_Of_Earth_George/fundamentals.html) |
| **Revision 2** | `blueprint.html` | **Blueprint & Educational Ecosystem Edition** (11-step sequence, 4 Pillars expansion) | [Open Revision 2](https://cmiller1466-ship-it.github.io/Being_Of_Earth_George/blueprint.html) |
| **Version 1** | `index.html` | **Baseline Flagship Front Door** (Initial movement-heavy baseline) | [Open Baseline](https://cmiller1466-ship-it.github.io/Being_Of_Earth_George/index.html) |

---

## 3. Mobile UI Polish & Layout Fixes
* **Diagnostic Step Indicator (Loom Review Fix):** On narrow mobile screens (360px–420px), the unstyled progress text collided with inline step numbers (`12 STEP 1 OF 3: YOUR PRIMARY HEALTH & 3 PAIN POINT`).
* **Dedicated CSS Design Tokens:** Added `.diag-step-indicator`, `.step-dot` (28x28 circular badge with gold active glow), `.step-line` (connector bar), and `.step-status-text`.
* **Mobile-First Layout:** On screens under 640px, the progress bar now stacks vertically (`flex-direction: column; align-items: flex-start; gap: 0.75rem;`), placing the circular numbered sequence above the uppercase step status for a clean, spacious mobile presentation.
* **Cache-Buster:** Bumped to `style.css?v=2.6` across all HTML files to ensure instant edge and browser cache invalidation.

