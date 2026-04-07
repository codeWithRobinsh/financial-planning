# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

MyFinance is a personal static HTML/CSS financial planning dashboard with two pages:
- **`index.html`** — Debt foreclosure plan tracking 5 active loans (₹10.65L total) with a 5-phase closure strategy targeting debt-free status by Jan 2027
- **`income-plan.html`** — Extra income roadmap targeting ₹30K–50K/month via freelancing, mentoring, content creation, and SaaS

## Running Locally

No build process — open directly or serve statically:

```bash
python3 -m http.server 8000
# Then open http://localhost:8000
```

## Architecture

**Zero-dependency static site** — pure HTML5 + CSS3, no JavaScript framework, no package manager.

Stylesheet split:
- `index.css` — shared base styles (typography, layout, CSS variables, component primitives)
- `income-plan.css` — income-page-specific styles (phase cards, schedule grid, projections table)

**CSS design tokens** (defined in `index.css` `:root`): purple primary (`#8b5cf6`), green success, red danger, orange warning, cyan info, light-gray background.

Both HTML files use:
- Native `<details>/<summary>` for collapsible sections
- SVG inline icons for bank/finance symbols
- CSS Grid + Flexbox for layout
- Google Fonts (Poppins, Fira Code)

## Data

All financial data is **hardcoded inline** in the HTML. There is no JSON data layer, no JavaScript calculations, and no backend. To update figures (loan balances, EMI amounts, dates), edit the HTML directly.

Supporting source documents are in [`Statements/`](Statements/) (PDFs and Excel).
