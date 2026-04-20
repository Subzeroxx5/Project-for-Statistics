# Project-for-Statistics

An interactive statistics simulation hosted on GitHub Pages.

## Live Simulation

**[Click to launch the Central Limit Theorem simulation](https://subzeroxx5.github.io/Project-for-Statistics/simulation.html)**

## Contents

| File | Description |
|---|---|
| `simulation.html` | Self-contained interactive CLT simulation (HTML + JS, no build step needed) |
| `report.tex` | LaTeX report that links to the hosted simulation via `\href{...}{Click to launch}` |
| `.github/workflows/pages.yml` | GitHub Actions workflow that deploys the repo to GitHub Pages on every push to `main` |

## LaTeX usage

The `report.tex` file uses the `hyperref` package to embed a clickable link:

```latex
\href{https://subzeroxx5.github.io/Project-for-Statistics/simulation.html}{Click to launch}
```

This works in any PDF viewer and avoids the need to embed raw HTML inside a
LaTeX/PDF document, which is not universally supported.

## Enabling GitHub Pages

1. Go to **Settings → Pages** in this repository.
2. Under *Source*, select **GitHub Actions**.
3. The next push to `main` will trigger the `pages.yml` workflow and publish the site.
