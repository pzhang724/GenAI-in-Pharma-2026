# GenAI-in-Pharma-2026

GenAI in Pharma 2026 — Virtual. A reveal.js presentation built with [Quarto](https://quarto.org).

- **Source:** [`Pre-GenAI-in-Pharma-2026.qmd`](Pre-GenAI-in-Pharma-2026.qmd)
- **Outline / scratch notes:** [`draft.md`](draft.md)
- **Live slides:** https://pzhang724.github.io/GenAI-in-Pharma-2026/Pre-GenAI-in-Pharma-2026.html
  (the repo root URL redirects here)

## How publishing works

Every push to `main` triggers `.github/workflows/publish.yml`, which renders the
Quarto project to `_site/` and deploys it to GitHub Pages. No `gh-pages` branch —
it uses the GitHub Actions Pages deployment.

### One-time setup (required before the first deploy works)

In the GitHub repo: **Settings → Pages → Build and deployment → Source → "GitHub Actions"**.

Until that source is set to GitHub Actions, the `deploy` job will fail with a
permissions/Pages-not-enabled error even though the render succeeds.

## Render locally (optional)

Requires [Quarto](https://quarto.org/docs/get-started/) installed.

```bash
quarto preview Pre-GenAI-in-Pharma-2026.qmd   # live reload while editing
quarto render                                  # build _site/
```
