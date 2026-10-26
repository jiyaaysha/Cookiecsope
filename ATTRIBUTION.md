# Attribution & Credits — Cookiescope

This file tracks every external resource (code, data, docs, design assets) used in the project, separated from what is original work. Keep this updated as the project grows — it protects you legally and makes due-diligence/investor review faster.

---

## 1. Third-Party Datasets

| Resource | Source / Owner | License | Used for | Link |
|---|---|---|---|---|
| Tracker/cookie identification list | *e.g. Disconnect.me Tracking Protection List* | *e.g. GPLv3 — check before commercial use* | Matching cookie domains to known trackers (Meta, Google, TikTok, etc.) | *add link* |
| *(add any paid threat-intel feed here)* | | | | |

> ⚠️ Action needed: confirm the license of any tracker list before using it commercially. Some (e.g. EasyList/EasyPrivacy) are free for most uses but require attribution; some commercial threat-intel feeds restrict redistribution of their data in your own paid product.

---

## 2. Third-Party Code / Libraries

| Library | Source | License | Used for |
|---|---|---|---|
| Puppeteer / Playwright | Google / Microsoft (open source) | Apache 2.0 / MIT | Headless browser automation for live site scanning |
| *(add any npm/pip packages used in the real MVP)* | | | |

---

## 3. Fonts & Design Assets

| Asset | Source | License | Used for |
|---|---|---|---|
| Inter | Google Fonts (Rasmus Andersson) | SIL Open Font License 1.1 | Body/UI typeface |
| IBM Plex Mono | Google Fonts (IBM) | SIL Open Font License 1.1 | Data/technical labels |

---

## 4. Documentation & External References Consulted

| Resource | Author/Owner | Used for |
|---|---|---|
| Chrome Extensions API docs (`chrome.cookies`, `chrome.webRequest`) | Google/Chromium project | Reference for extension architecture (no code copied) |
| Cookiebot / OneTrust public pricing pages | Respective companies | Market/pricing benchmarking only — no content reused |

---

## 5. Original Implementation (built for Cookiescope specifically)

- Visual design system, layout, and copywriting on the demo website
- Risk-tier categorization logic (Essential / Functional / Analytics / Advertising / Harmful)
- The "X-ray / radiography" product concept, scan interaction, and UI components
- Discrepancy-detection framing (comparing banner language to actual data behavior)
- All business/pricing/go-to-market content drafted in planning docs

---

## How to Use This File

- Add a row **every time** you bring in an external library, dataset, font, icon set, or copy-paste code from a tutorial/Stack Overflow.
- Before using any dataset commercially, check its license — "free to view" is not the same as "free to redistribute inside a paid product."
- Keep this file in your code repository root (`ATTRIBUTION.md` or `CREDITS.md`) so it's visible to collaborators, auditors, and potential investors doing due diligence.
