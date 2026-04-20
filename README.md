# Varshit Manepalli — Portfolio

> Personal portfolio website for a GenAI & ML Engineer. Built as a production-grade static site with a dark-first design system, animated neural network canvas, scroll-reveal animations, and a live contact form backed by Web3Forms.

**Live:** [varshitmanepalli.github.io/portfolio](https://varshitmanepalli.github.io/portfolio/)

---

## Overview

Single-page portfolio covering:

- **Hero** — animated neural network background, profile photo, key stats
- **About** — bio, education (Stevens Institute of Technology M.S. CS, VIT-AP B.Tech), certifications
- **Experience** — vertical timeline across 5 roles (Okada & Company, Escape™ App AI, Progress Solutions, Stevens Research, Divami)
- **Projects** — 7 ML/AI projects with images, tech stacks, and GitHub links
- **Skills** — 6 grouped categories with animated expertise depth bars
- **Contact** — live email delivery via Web3Forms (no backend required)

---

## Tech Stack

| Layer | Choice |
|---|---|
| Markup | Semantic HTML5 |
| Styling | Vanilla CSS with custom design tokens (no framework) |
| Typography | Clash Display · Satoshi · JetBrains Mono (via Fontshare + Google Fonts) |
| Animation | CSS keyframes + IntersectionObserver scroll-reveal |
| Canvas | Vanilla JS neural network particle system |
| Email | [Web3Forms](https://web3forms.com) API (250 free submissions/month) |
| Hosting | GitHub Pages |

---

## Project Structure

```
portfolio/
├── index.html                  # Single-page application (all sections)
├── assets/
│   └── images/
│       ├── profile/
│       │   └── varshit-manepalli.jpg     # Profile photo
│       └── projects/
│           ├── ai-soundscapes.jpg
│           ├── cyberattack-gan-detection.jpg
│           ├── hate-speech-detection.jpg
│           ├── hedge-fund-simulator.jpg
│           ├── hiv-therapy-optimization.jpg
│           └── weather-forecasting.jpg
└── README.md
```

---

## Running Locally

```bash
git clone https://github.com/varshitmanepalli/portfolio.git
cd portfolio
# Open directly — no build step required
open index.html
```

Or with a local dev server (recommended for accurate asset loading):

```bash
npx serve .
# → http://localhost:3000
```

---

## Design System

The site uses a custom CSS design token system — no Tailwind, no external CSS framework.

| Token group | Details |
|---|---|
| `--color-bg` / `--color-surface` | Deep navy dark mode (`#080c14` / `#0d1220`) |
| `--color-primary` | Electric cyan `#00d4ff` |
| `--color-secondary` | Soft purple `#9d7aea` |
| `--font-display` | Clash Display (headings) |
| `--font-body` | Satoshi (body text) |
| `--font-mono` | JetBrains Mono (labels, tags, code) |
| `--text-*` | Fluid type scale via `clamp()` |

Dark/light mode toggle is built-in (`data-theme` attribute on `<html>`).

---

## Contact Form

The form POSTs to the [Web3Forms](https://web3forms.com) API:

- No backend or server required
- Emails delivered directly to `varshitmanepalli1810@gmail.com`
- Honeypot field (`botcheck`) for spam protection
- Async fetch with inline success/error states — no page redirect

---

## License

MIT — feel free to fork and adapt for your own portfolio.
