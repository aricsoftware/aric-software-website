# ARIC Software & Design, Inc — Website

Mobile-first, single-page marketing website for **ARIC Software & Design, Inc** (DBA **ARIC Software** and **ARIC Enterprise Solutions**).

## Tech Stack

| Layer | Choice | Why |
|-------|--------|-----|
| Markup | HTML 5 | Semantic, accessible |
| Styling | **Tailwind CSS v4** (CDN) | Utility-first, mobile-first by default, zero build step |
| JS | Vanilla ES6 | Lightweight — no framework overhead for a marketing page |

## Quick Start

```bash
# Option 1 — just open the file
open index.html          # macOS

# Option 2 — local dev server (requires Python 3)
cd aric-software-website
python3 -m http.server 8000
# then visit http://localhost:8000

# Option 3 — VS Code Live Server extension
# Right-click index.html → "Open with Live Server"
```

## Structure

```
aric-software-website/
├── index.html   # Full single-page site (HTML + Tailwind + JS)
└── README.md    # This file
```

## Sections

- **Navbar** — responsive, mobile hamburger menu, sticky with blur backdrop
- **Hero** — gradient banner with CTAs
- **Services** — 6-card grid (software dev, enterprise, design, cloud, mobile, security)
- **About** — brand story (parent + two DBAs) with stat cards
- **Solutions** — ARIC Enterprise Solutions showcase
- **Contact** — form + company info
- **Footer** — legal name, DBAs, nav links, copyright

## Customization

- **Brand colors** — edit `tailwind.config` inside `<script>` in `index.html` (`brand` palette)
- **Content** — all text is inline in `index.html`
- **Contact form** — currently client-side only; wire the `<form>` action to your backend or a service like Formspree / Netlify Forms

## License

© ARIC Software & Design, Inc. All rights reserved.
