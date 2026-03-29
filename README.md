# Verbatim

**A Wall of Words** — an infinite, scrollable masonry mosaic of the world's greatest quotes.

## What it is

Verbatim is a Progressive Web App (PWA) that displays hundreds of curated quotes in a living, typographic wall. Quotes are rendered in 12 different Google Fonts, arranged in a true masonry grid, and refresh with a card-flip animation every 15–40 seconds.

## Features

- **True masonry layout** — 12 columns, each tile's height driven by its content
- **Bidirectional scroll** — pan horizontally and vertically across 3600px of quotes
- **Pinch to zoom** — 100% (12 cols overview) → 150% (8 cols zoomed in)
- **Card-flip animation** — tiles in view refresh with new quotes every 15–40s
- **Live quote APIs** — quotable.io, quote-garden, zenquotes (186 built-in fallback)
- **12 Google Font voices** — Playfair Display, Oswald, Bebas Neue, Abril Fatface, Cormorant Garamond, and more
- **Shuffle** — rebuilds the wall with a new random layout
- **Share / Copy** — native share sheet on mobile, clipboard on desktop
- **PWA** — installable on Android and iOS, works offline
- **Difference-mode cursor** — always visible regardless of tile background color

## Tech

Pure HTML + CSS + JS. No framework, no build step, no dependencies.

## Deploy

### Netlify (drag and drop)
1. Go to [netlify.com](https://netlify.com)
2. Drag this folder onto the deploy zone
3. Done

### Vercel (from GitHub)
1. Import this repo at [vercel.com](https://vercel.com)
2. No build command needed, output directory is `/`
3. Deploy

### Local dev
```bash
python3 -m http.server 8080
# open http://localhost:8080
```

> Note: Must be served over HTTP/HTTPS for PWA features (service worker, manifest). Opening `index.html` directly via `file://` will work for the visual but not PWA install or live APIs.

## License

MIT
