# Travel SOS — React

A standalone React port of the Travel SOS prototype. Same design, screens, flows,
Arabic/English UI with RTL, the Language Help translation demo, and all mock data.
No backend, no real APIs, no OCR, no real payments — everything is simulated, as in
the original.

## Run locally

```bash
npm install
npm run dev
```

## Build for deployment

```bash
npm run build
```

This produces a static `dist/` folder you can deploy to Netlify, Vercel, Cloudflare
Pages, GitHub Pages, or any static host — just upload/point the host at `dist/`.

## What's inside

- `src/screens/` — one component per app screen (Home, My Trip, SOS, Analysis,
  Action Plan, Talk/Language Help, Airport Navigation, Cases, Profile, Pass)
- `src/context/AppContext.jsx` — all app state (language, active trip, current
  problem, cases, pass status) and the actions that drive navigation, mirroring
  the original app's logic
- `src/data/problems.js` — the bilingual problem/guidance/case data
- `src/utils/talkEngine.js` — the local, rule-based Arabic↔English demo
  translator used by Language Help (no external service)
- `src/i18n/strings.js` — UI chrome text (nav, headings, buttons) in both languages
- `src/styles.css` — the original visual design, unchanged
