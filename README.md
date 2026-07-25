# AverixAI Website

A fully static, responsive 4-page website for AverixAI — a nonprofit teaching teens practical AI skills through mentorship and real-world projects. Built with plain HTML5, CSS3, and vanilla JavaScript only (no frameworks, no build step), so it can be hosted directly on GitHub Pages.

## Structure

```
AverixAI/
├── index.html       Home — hero, about summary, program overview, testimonials
├── about.html        Mission, stats, leadership board, values
├── events.html        Past + upcoming events
├── programs.html      Full curriculum, highlights, timeline, apply CTA
├── style.css          Shared design system (colors, type, components)
├── script.js           Mobile nav, scroll reveal animations, stat counters
├── images/
│   └── logo.png        AverixAI logo
└── README.md
```

## Design system

- **Colors:** Navy `#0B3C6F`, Light Blue `#2FA8DC`, White, Light Gray `#F8FAFC`
- **Type:** Poppins (headings) + Inter (body), loaded from Google Fonts
- **Signature motif:** a dotted "synapse" line — echoing the brain → circuit mark in the logo — used for section dividers, the animated hero graphic, and timeline connectors
- **Motion:** scroll-triggered fade/slide reveals, animated stat counters, hover lifts — all respect `prefers-reduced-motion`

## Running locally

No build step required. Open `index.html` directly in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploying to GitHub Pages

1. Push this folder to a GitHub repository.
2. In the repo settings, enable GitHub Pages and point it at the root of the `main` branch.
3. Your site will be live at `https://<username>.github.io/<repo-name>/`.

## Customizing

- **Photos:** replace the dashed circular placeholders in `about.html` (leadership cards) and the gradient blocks used for the hero/about/program imagery with real photography.
- **Events:** duplicate `.event-card` blocks in `events.html` as new events are added.
- **Copy:** all headline and body copy lives directly in the HTML files — no CMS or data file required.
