# Being of Earth — Phase 1 Static Front Door

Official static front-door website for **Being of Earth** (George Chountalos), engineered by Cenote Softworks.

* **Stack:** Pure semantic HTML5 + CSS3 (No runtime JS frameworks, zero telemetry)
* **Design Standard:** Cenote Softworks UI Standard (`CENOTE_UI_STANDARD.md` — Theme 3: Warm Humanist Heritage)
* **Hosting:** Cloudflare Pages (Static Edge, $0/mo)
* **Target Domain:** `www.beingofearth.com` & `beingofearth.com`
* **Course & Member Portal Engine:** GoHighLevel (`go.beingofearth.com`)
* **Support Email:** `info@beingofearth.com`
* **Direct Support / WhatsApp:** `+52 999-551-8626`

---

## Project Structure

```
├── assets/
│   ├── icons/       # Brand logos and vector badges
│   ├── images/      # Kinesiology photos, guides, testimonials
│   └── video/       # Full-bleed nature video hero loop (10.9 MB)
├── docs/
│   └── PHASE_1_BLUEPRINT.md  # Architectural roadmap and funnel specs
└── src/
    ├── index.html   # Main long-form conversion page
    └── style.css    # 8px spatial grid, WCAG AA compliant theme
```

---

## Deployment to Cloudflare Pages

1. **Framework Preset:** None (Static HTML)
2. **Build Command:** None
3. **Build Output Directory:** `.` or `dist` (if bundling)
4. **Custom Domains:** `www.beingofearth.com`, `beingofearth.com`
