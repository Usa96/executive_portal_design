# SANAM Executive Portal — Design v3

Front-end redesign of the SANAM Executive Portal, built as a single interactive
artboard in the sanam.com visual language. Prototype only — the live codebase
(`Usa96/Executive_Portal`) is untouched.

Live canvas: https://claude.ai/artifact/FXxbzDrRSrr6KHw9xBKtWW

## Layout

```
design/project/Main.dc.html   the artboard — markup, styles and logic in one file
design/project/canvas.json    canvas index (one fluid artboard, launches focused)
assets/images/                entity and platform photography (resized)
assets/logos/                 SANAM, Eradat, Abyan, ERMC, TIAC, NATMED, MEDCAP, Spirit, MADAREK
assets/video/                 hero video (sanam.com title video)
docs/screens/                 rendered screenshots at 1440 / 1024 / 800 / 390
```

Image references inside `Main.dc.html` are `/_blob/<id>` asset URLs from the
canvas; the same files sit under `assets/` for porting.

## Screens

Workspace · Platform · Entity · Folder · All documents · Structure (org chart) ·
Budget (consolidated + per-entity) · Access matrix · People · Audit trail.

## Visual system

- Colours: dark `#21201f`, taupe `#bdaba2`, light `#f6f1f0`
- Type: Helvetica Neue
- Breakpoints: 1280 (hamburger nav), 1100 (2-col grids), 760 (single column)

## Structure

4 platforms → 16 grantable entities (11 companies + 5 MADAREK schools).
Real Estate is one company, Eradat, carrying the 7 Kuwait properties as assets
(no folders, no separate budget).

## Preview site

`site/` is a self-contained static build of the artboard (page, runtime, assets).
`.github/workflows/pages.yml` deploys it to GitHub Pages on every push to `main`.
Enable Pages once: repo **Settings → Pages → Source: GitHub Actions**.
