# Lifeline Emed — Website (v4)

Marketing & scholarly-publishing website for **Lifeline Emed Companies LLC**, official publisher of the **American Journal of Research & Innovation (AJRI)**.

A static, multi-page site built with plain HTML, CSS, and JavaScript — no build step required.

## Features

- **Light, clean theme** with a navy + gold academic identity
- **Full-bleed dark hero** with the NYC skyline, parallax depth, and a gold progress bar
- **Smooth inertia scrolling** via [Locomotive Scroll](https://github.com/locomotivemtl/locomotive-scroll) (self-hosted), with native-scroll fallback on mobile and for `prefers-reduced-motion`
- **Staggered scroll-reveal** animations
- Shared **nav + footer** injected by `assets/main.js` (single source of truth across all pages)
- Fully **responsive** (centered menu collapses to a hamburger on small screens)

## Pages

| Page | File |
| --- | --- |
| Home | `index.html` |
| About | `about.html` |
| Journals (AJRI) | `journals.html` |
| Research Areas | `research-areas.html` |
| Editorial Board | `editorial-board.html` |
| Conferences | `conferences.html` |
| Publications | `publications.html` |
| Contact | `contact.html` |
| Sign Up / Login | `signup.html`, `login.html` |
| Legal | `privacy-policy.html`, `terms-of-service.html`, `cookie-policy.html`, `disclaimer.html`, `accessibility-statement.html` |

## Project structure

```
.
├── index.html, about.html, … (pages)
└── assets/
    ├── styles.css            # design system + all styles
    ├── main.js               # shared nav/footer, scroll behavior, Locomotive init
    ├── hero-city.jpg         # hero background
    └── vendor/               # self-hosted Locomotive Scroll
```

## Run locally

Any static file server works, e.g.:

```bash
python -m http.server 5500
# then open http://localhost:5500
```

## Notes

- Contact / auth forms are front-end only (demo) — no backend is connected.
- Content is for the AJRI inaugural volume (Vol. 1, 2026): ISSN pending, DOI planned.
