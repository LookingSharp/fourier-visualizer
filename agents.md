# Agent Guide

## Project
Static HTML Fourier visualizer deployed to GitHub Pages.  
Live: https://lookingsharp.github.io/fourier-visualizer/index.html

## Structure
| File | Purpose |
|------|---------|
| `index.html` | Landing page — JS detects mobile/desktop and redirects |
| `fourier-visualizer.html` | Desktop version (sidebar layout) |
| `fourier-visualizer-mobile.html` | Mobile version (tab navigation, touch-optimized) |

## Key Facts
- **No build system.** Pure HTML/CSS/JS — no npm, no bundler, no compiler.
- **All CSS and JS are inline** inside each HTML file. There are no separate `.js` or `.css` files.
- **No test suite, no linter** configured.
- Merging to `main` auto-deploys via `.github/workflows/static.yml` (GitHub Pages).

## On Every PR
Evaluate whether your changes require an update to `agents.md`.
