# Financial Planning Dashboard

A comprehensive personal finance dashboard for debt management and income planning.

## Live Demo

🔗 [View Dashboard](https://codewithrobinsh.github.io/financial-planning/)

## Features

### 📊 Debt Foreclosure Planner (`index.html`)
- **Portfolio Overview** — Track 5 active loans totaling ₹10.65L with real-time progress indicators
- **Optimized Foreclosure Strategy** — 5-phase plan targeting debt-free status by Jan 2027
- **Interest Savings Calculator** — Save ₹62,109 via strategic early closures
- **Monthly Cash Flow Projections** — Detailed inflow/outflow timeline
- **Penalty Analysis** — Smart recommendations on when to foreclose vs let loans mature naturally

### 💰 Extra Income Roadmap (`income-plan.html`)
- **Phased Income Growth** — Target ₹30K–₹50K/month extra income
- **Multiple Income Streams** — Mentoring, freelancing, courses, micro-SaaS
- **Weekly Time Budget** — 39 hours/week allocation strategy
- **Realistic Projections** — Month-by-month income growth estimates
- **Action Plan** — Prioritized steps to start earning immediately

## Tech Stack

- **HTML5** — Semantic markup with collapsible sections (`<details>/<summary>`)
- **CSS3** — Custom properties, Grid, Flexbox, gradients, animations
- **Google Fonts** — Poppins (body), Fira Code (numbers)
- **Zero JavaScript** — Pure CSS interactivity
- **Responsive Design** — Mobile-first with breakpoints at 480px, 768px, 1024px

## Screenshots

### Debt Foreclosure Dashboard
![Debt Plan](https://via.placeholder.com/800x400?text=Debt+Foreclosure+Dashboard)

### Income Roadmap
![Income Plan](https://via.placeholder.com/800x400?text=Income+Roadmap)

## Project Structure

```
├── index.html          # Debt foreclosure dashboard
├── index.css           # Shared styles + debt page styles
├── income-plan.html    # Extra income roadmap
├── income-plan.css     # Income page specific styles
├── CLAUDE.md           # AI assistant context
└── Statements/         # Source documents (PDFs, Excel)
```

## Color Palette

| Token | Hex | Usage |
|-------|-----|-------|
| Primary | `#8b5cf6` | Purple accents, links |
| Success | `#22c55e` | Positive values, savings |
| Danger | `#f43f5e` | Outstanding amounts, warnings |
| Warning | `#f97316` | Caution indicators |
| Info | `#0ea5e9` | Informational badges |

## Running Locally

No build process required — just serve the files:

```bash
# Using Python
python3 -m http.server 8000

# Using Node.js
npx serve .

# Then open http://localhost:8000
```

## Data

All financial data is **hardcoded inline** in HTML. To update figures (loan balances, EMI amounts, dates), edit the HTML directly. No JSON data layer or JavaScript calculations.

---

**Disclaimer:** This dashboard is for personal planning purposes only and does not constitute financial advice.

© 2026 Financial Planning · Built by Robinsh Kumar