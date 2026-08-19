# amco100.me — The Prompt Architect

Static site, served by GitHub Pages from `main`. No build step, no dependencies,
no external requests: plain HTML and one stylesheet.

- `index.html` — home and post list
- `writing/` — one file per post
- `about.html`, `404.html`, `style.css`
- `CNAME` — the custom domain

⚠ **The CNAME file is load-bearing and was wrong for nine days.** It read
`amco1000.me` (three zeros) while the registered domain is `amco100.me` (two).
GitHub Pages served the site on the typo domain and returned 404 on the real
one. Both domains resolve to Pages, so DNS looked healthy the whole time — the
only symptom was the 404. If the site goes dark, check this file first.
