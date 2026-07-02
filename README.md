# Swisscard Executive Demo

Interactive story deck — **Acquisition · Retention · Referral** (Act 03 Deepening hidden in presenter mode).

**Live demo:** [https://zkorczyc.github.io/swisscard-demo/](https://zkorczyc.github.io/swisscard-demo/)

Navigate with **← →**, **space**, or **click**. Jump to a slide with **`#18`** (1-based, visible slides only — hidden deepening slides are skipped).

---

## Preview locally

```bash
python3 -m http.server 8080
# Open http://localhost:8080
```

## Four acts

| Act | Persona | Tagline |
|---|---|---|
| **01 Acquisition** | Marc Weber | Win the right customer |
| **02 Retention** | Sofia Müller · Amex Gold | Win back with relevance |
| **03 Deepening** | Marc Weber | *(hidden in deck)* Grow every relationship |
| **04 Referral** | Marc → Lukas | Close the loop |

**Practitioner:** Claudia Meier (all acts)

## Deploy (GitHub Pages)

This repo **is** the site — `index.html` at the root, no build step.

1. Push to `main` on [zkorczyc/swisscard-demo](https://github.com/zkorczyc/swisscard-demo).
2. **Settings → Pages** → Source: **Deploy from branch** → `main` → **`/ (root)`**.
3. Wait ~1–2 minutes. Site: `https://zkorczyc.github.io/swisscard-demo/`

`.nojekyll` is included so GitHub Pages serves assets as-is.

## Repository layout

| Path | Purpose |
|---|---|
| `index.html` | Self-contained interactive deck |
| `assets/` | Persona portraits, device mocks, creatives |
| `adobe-wordmark-red.svg` | Footer wordmark |

Planning docs (story, steps, validations) live in the parent monorepo under `swisscard/` — not required to run the deck.

## Maintenance notes

- **Act 03 Deepening:** slides use class `slide-hidden` — remove to restore in navigation.
- Replace remaining `img-ph` placeholders with Adobe UI screenshots when ready.
