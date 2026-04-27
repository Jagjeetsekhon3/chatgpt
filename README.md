# Sekhon Designer Freelance Website

Simple responsive one-page freelance portfolio website for **www.sekhondesigner.com**.

## Files
- `index.html` – page structure and content
- `styles.css` – styling and responsive layout
- `script.js` – mobile menu toggle and dynamic footer year
- `vercel.json` – explicit static build + fallback route config for Vercel

## Run locally
```bash
python3 -m http.server 8000
```
Then open `http://localhost:8000`.

## Vercel fix for 404
This repository now includes an explicit Vercel static build config.

If you still see `404: NOT_FOUND`, check Vercel Project Settings:
- **Root Directory** → repository root (where `index.html` exists)
- **Framework Preset** → Other
- **Build Command** → empty
- **Output Directory** → empty
- Then click **Redeploy** (clear build cache if prompted)

`vercel.json` forces static builds for `index.html`, `styles.css`, and `script.js`, then routes unknown paths to `index.html`.

## Customize quickly
- Update hero/about text in `index.html`
- Replace portfolio cards with real project details and links
- Update contact form behavior by connecting it to a backend service
