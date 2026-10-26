# Cookiescope

A browser forensics tool that X-rays any website's cookies before you click "accept," flagging exactly which trackers are active and where your data actually goes. Built for fintech teams who need to prove — not just promise — that their consent banners match their real data practices.

![status](https://img.shields.io/badge/status-prototype-blueviolet)
![license](https://img.shields.io/badge/license-MIT-brightgreen)

## What this is

This repo currently contains the **front-end prototype / demo** — a static, interactive mockup showing the full product experience with sample scan data. It is not yet wired up to a real scanning backend. See [Roadmap](#roadmap) below for what a production version needs.

## Features (demo)

- Simulated "scan" interaction with an animated X-ray plate visual
- Cookie inventory grouped into five risk tiers: **Essential, Functional, Analytics, Advertising, Harmful/Fingerprinting**
- Filterable table (all / shared-with-third-parties / fingerprinting-only)
- Discrepancy callout comparing a site's stated consent language against actual tracking behavior
- Fully responsive, light pastel UI with accessible focus states and reduced-motion support

## Tech stack

- Plain HTML / CSS / vanilla JavaScript — no build step, no dependencies
- Fonts: [Inter](https://fonts.google.com/specimen/Inter) and [IBM Plex Mono](https://fonts.google.com/specimen/IBM+Plex+Mono) via Google Fonts

## Getting started

No installation needed — it's a single static file.

```bash
git clone https://github.com/<your-username>/cookiescope.git
cd cookiescope
open index.html   # or just double-click it / drag into a browser
```

To serve it locally instead of opening the file directly:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Project structure

```
cookiescope/
├── index.html        # the full front-end prototype
├── README.md          # this file
├── ATTRIBUTION.md      # credits for fonts, libraries, and datasets used
└── LICENSE
```

## Roadmap

- [ ] Replace mock scan data with a real headless-browser scanner (Puppeteer/Playwright)
- [ ] Integrate a tracker-identification dataset (e.g. Disconnect.me / EasyPrivacy lists) — see `ATTRIBUTION.md` before using any list commercially
- [ ] Build a backend API to run and store scans
- [ ] User accounts + scheduled re-scans
- [ ] PDF/exportable compliance reports
- [ ] Browser extension (real-time, in-session scanning)

## Credits

External fonts, libraries, and datasets referenced or planned for use are tracked in [`ATTRIBUTION.md`](./ATTRIBUTION.md), kept separate from original project work.

## License

MIT — see [`LICENSE`](./LICENSE).
