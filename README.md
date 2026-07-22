# Indicivics

A bilingual civics education site for India, deployed as a single self-contained static page.

**Live site:** https://indicivics.com

## What it is

An interactive, mobile-first civics learning experience covering how India is governed. Content is available in:

- **English**
- **Hindi (हिंदी)**
- **GenZ tone mode** — the same civics content, rephrased in a casual, Gen-Z register

The experience is structured as **six learning modules** followed by a **final quiz**, which generates a **shareable result poster** at the end.

## How it's built

- A single `index.html` (~5 MB) — a fully self-contained static bundle.
- **No build step.** It is served exactly as-is.
- **No external dependencies at runtime:** all fonts are base64-embedded, and all scripts (including the React runtime) are inlined into the page. Loading the page makes zero remote network requests.

## Deployment

Hosted on **GitHub Pages** from the `main` branch (root), with `indicivics.com` set as the custom domain via the `CNAME` file. To update the site, edit `index.html` and push to `main`; GitHub Pages redeploys automatically.

## Repository layout

| File | Purpose |
|------|---------|
| `index.html` | The entire website — self-contained bundle |
| `CNAME` | Custom domain for GitHub Pages (`indicivics.com`) |
| `.gitignore` | Ignores OS/editor cruft |
| `README.md` | This file |
