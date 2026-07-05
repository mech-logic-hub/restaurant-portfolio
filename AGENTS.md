# AGENTS.md

## Cursor Cloud specific instructions

This repository is a **pure static HTML site** (a restaurant landing-page portfolio, Japanese). Key facts for future agents:

- There is **no build step, no package manager, and no dependencies to install**. There is no `package.json`, `requirements.txt`, `Makefile`, or lockfile. Do not attempt to run `npm`/`pip`/etc.
- There is **no lint or automated test tooling**. The only CI check (`.github/workflows/pages.yml`) just verifies that the four HTML files exist (`index.html`, `warm/index.html`, `wa-modern/index.html`, `machi-shokudo/index.html`) before deploying to GitHub Pages.
- **Run / preview locally** (from repo root): `python3 -m http.server 8080`, then open `http://localhost:8080/`. Any port works; nothing is hardcoded. Serving from the repo root is required so the relative links (`warm/`, `wa-modern/`, `machi-shokudo/`) resolve like on GitHub Pages.
- Content: one 5-block LP template rendered in 3 visual themes for a fictional restaurant. Images are Unsplash placeholders and Google Fonts are loaded via CDN, so full visual rendering needs network access.
