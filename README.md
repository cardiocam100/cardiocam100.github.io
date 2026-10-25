# amco100.me — The Prompt Architect

Static site, served by GitHub Pages from `main`. No build step, no dependencies,
no external requests: plain HTML and one stylesheet.

- `index.html` — the AMCO home page: a scroll-driven motion film (GSAP, one
  timeline). BUILT, do not hand-edit: source lives in Asset-Orchestrator
  `docs/amco-site/` (`node build.mjs`), then copy `dist/index.html` and
  `dist/assets/` here.
- `assets/` — fonts (OFL, licences alongside), gsap.min.js, scene images
- `writing/` — the blog: `writing/index.html` is the post list, one file per post
- `about.html`, `404.html`, `style.css`
- `CNAME` — the custom domain

⚠ **The CNAME file is load-bearing and was wrong for nine days.** It read
`amco1000.me` (three zeros) while the registered domain is `amco100.me` (two).
GitHub Pages served the site on the typo domain and returned 404 on the real
one. Both domains resolve to Pages, so DNS looked healthy the whole time — the
only symptom was the 404. If the site goes dark, check this file first.
