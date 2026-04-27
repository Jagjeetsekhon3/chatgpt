# Sekhon Designer Freelance Website

Simple responsive one-page freelance portfolio website for **www.sekhondesigner.com**.

## Files
- `index.html` – page structure and content
- `styles.css` – styling and responsive layout
- `script.js` – mobile menu toggle and dynamic footer year
- `vercel.json` – Vercel routing so all paths load `index.html`

## Run locally
```bash
python3 -m http.server 8000
```
Then open `http://localhost:8000`.

## Vercel fix for 404
If Vercel shows `404: NOT_FOUND`, ensure:
- Root Directory is the repository root (where `index.html` exists)
- Framework Preset is set to **Other**
- `vercel.json` is committed (already included in this repo)

This config rewrites all routes to `index.html`, so direct links like `/portfolio` still work.

## Customize quickly
- Update hero/about text in `index.html`
- Replace portfolio cards with real project details and links
- Update contact form behavior by connecting it to a backend service
