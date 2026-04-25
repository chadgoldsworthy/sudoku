# Sudoku

A modern, mobile-first Sudoku web app. Single self-contained HTML file — no build, no dependencies.

Live: `https://<your-username>.github.io/<repo-name>/`

## Features

- Unlimited puzzles via an in-browser generator (unique-solution checked)
- Five difficulties: Easy, Medium, Hard, Extra hard, Expert
- Pen, Pencil, and Eraser tools
- Hints with a two-step explanation (technique → exact placement)
- Smart highlights: peers, same-number, conflicts
- Light and dark themes
- Local stats dashboard: totals, per-difficulty best/avg, recent games
- Win detection with summary
- Theme + settings + stats persisted in `localStorage`
- Keyboard support (1–9, arrows, Backspace)

## Run locally

Just open `index.html` in any browser. Or, for a quick local server:

```sh
python3 -m http.server 8000
# then open http://localhost:8000/
```

## Deploy to GitHub Pages

1. Create a public repo on GitHub (e.g. `sudoku`).
2. Push this folder's contents (`index.html`, `README.md`) to the `main` branch.
3. In the repo: **Settings → Pages → Source: Deploy from a branch → Branch: main / root → Save**.
4. After ~1 minute, the app is live at `https://<your-username>.github.io/<repo-name>/`.
5. On your phone: open that URL in Safari/Chrome → Share → **Add to Home Screen**. It launches fullscreen like a native app.

## State persistence

All preferences and stats are stored locally on your device via `localStorage`. Nothing is sent to any server. State survives reloads and app restarts. On iOS Safari, "Add to Home Screen" makes storage more durable (avoids ITP eviction).

## Built with Claude Code
```zsh
claude --resume "SUDOKU GITHUB PAGE"
```
