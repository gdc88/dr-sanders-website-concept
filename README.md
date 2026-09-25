# Dr. Sanders — website concept

A discussion prototype for the planned redesign of `ingenieurbuero-sanders.de`.

**Status:** working concept, not approved for production publication.

## Purpose

This is deliberately a focused concept rather than a complete free website. It demonstrates:

- a clear first-screen proposition;
- services organised around client decisions;
- an evidence-led case-study pattern;
- explicit separation of verified, existing and still-to-confirm claims;
- a safe staged delivery narrative;
- responsive German, Russian and English content;
- an intentionally non-functional contact form path (only published telephone/email links).

## Design system

- **Surface:** Decide / Learn — one idea per section, supported by evidence.
- **Style:** editorial engineering; restrained, precise and personal.
- **Palette:** warm mineral paper, structural charcoal, one copper accent.
- **Typography:** narrow technical sans hierarchy with restrained serif numerals/monogram; system fonts only.
- **Layout:** asymmetric hero, indexed service ledger, evidence-led cases, no generic equal feature-card grid.
- **Motion:** minimal state feedback only; `prefers-reduced-motion` is respected.
- **Accessibility:** semantic landmarks, skip link, visible focus, 44px controls, descriptive image text, responsive breakpoints.
- **Avoided:** stock hero photography, AI-purple gradients, fake testimonials, invented legal text, unverified badges and decorative metrics.

## Source and evidence discipline

Visible project facts and images were taken from the client's existing public project archive solely for this redesign discussion:

- Ollenhauer Straße 35: `https://ingenieurbuero-sanders.de/portfolio-items/mehrfamilienhaus-ollenhauer-str-35-13403-berlin/`
- AMAZON logistics centre, Stade: `https://ingenieurbuero-sanders.de/portfolio-items/amazon-logistikzentrum-kuhweidenweg-5-21684-stade/`
- Geisbergstraße 6: `https://ingenieurbuero-sanders.de/portfolio-items/geisberg-str-6-10777-berlin/`

Before a production release, the client must confirm facts, roles, usage rights, qualifications, legal identity, chamber/certification/insurance wording, addresses, language scope and contact-processing terms.

No copied competitor layout, copy or source code is used.

## Privacy / indexing posture

- `<meta name="robots" content="noindex, nofollow, noarchive, nosnippet">`
- `robots.txt` disallows crawling.
- There is no analytics, cookie, external font, form backend or tracking script.
- This does **not** make a GitHub Pages URL private. Anyone with the URL can open it.

## Local preview

```bash
python3 -m http.server 8080
```

Open `http://127.0.0.1:8080/`.

## Files

- `index.html` — semantic page content
- `styles.css` — complete responsive visual system
- `script.js` — language switcher, responsive navigation and concept notice
- `assets/` — optimised existing project images used for discussion
- `robots.txt` — crawler exclusion request

## Production gate

This repository is a prototype. Connecting a production domain, activating forms, adding analytics or migrating content requires a separately approved scope, verified legal/privacy texts, tested backup/restore, redirects, DNS/email safeguards and a rollback plan.
