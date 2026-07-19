# MasApp

A mobile-first health & fitness tracker PWA. All markup, styles, and logic
live in [`index.html`](index.html); images and icons live in
[`assets/`](assets). There's no build step and no backend — data is
persisted locally in the browser via `localStorage`.

## Features

- **Home** — daily overview: calorie fuel gauge and protein / carbs / fat
  macro dials.
- **Food** — log meals and track calories and macros against your goals.
- **Supps** — supplement stack organized by phase (e.g. Morning, Before
  Bed) with per-item doses and "mark all taken".
- **Body** — body stats and progress tracking.
- **Gym** — workout / lifting logging.
- **Calendar** — training plan and schedule.
- **Coach** — guidance and insights.

## Getting started

There's nothing to install or build. Just open it (keep `index.html` and
the `assets/` folder together — the app loads its images from there):

```bash
open index.html          # macOS
# or double-click index.html in your file browser
```

To use it as an installable app on a phone, host the folder over HTTPS and
"Add to Home Screen" from your mobile browser — it's configured as a
standalone web app.

## Project structure

```
.
├── index.html   # the app: UI + styles + logic
├── assets/      # icons and images (app icon, brand logo, body figures)
└── README.md
```

## Development

Edit `index.html` directly and refresh the browser. Styles live in the
`<style>` block near the top; app logic is in the `<script>` block. Data
lives in `localStorage`, so clearing site data resets the app.
