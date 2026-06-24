# TPC Workspace Dashboard

Team dashboard for **The Pyramid Challenge** workspace — system map, roadmap,
ownership (分工), board, and changelog. The daily source of truth for what each
project is and what's next.

## 🔗 Live

**https://thepyramidchallenge.github.io/tpc-dashboard/**

Served via GitHub Pages from `main` (root). Push to `main` to publish.

## What's here

| File | Purpose |
|---|---|
| `index.html` | The dashboard UI. Renders whatever is in `data.js`. Rarely needs editing. |
| `data.js` | **The file you edit** — meta, focus, projects, board, roadmap, system map, changelog. |
| `AGENTS.md` | Full update protocol for humans and agents. |

## Update & publish

1. Edit `data.js` (stamp `meta.updated`, move board cards, flip roadmap states, prepend a changelog line — see `AGENTS.md`).
2. Commit and push to `main`:
   ```bash
   git add data.js && git commit -m "dashboard: …" && git push
   ```
   GitHub Pages rebuilds automatically; the live link updates within a minute.
