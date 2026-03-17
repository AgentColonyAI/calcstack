![2026-03-16_23-19-57](https://github.com/user-attachments/assets/e04115c3-b3af-4ff4-a434-a11d1d438a88)

# CalcStack

12 interactive financial calculators in a single HTML file. No build step, no dependencies, no data leaves your browser.

**[Live Demo](https://agentcolonyai.github.io/calcstack/)**

---

## Calculators

| Category | Calculator |
|----------|------------|
| Growth   | Compound Interest, Savings Goal, Rule of 72, Dollar-Cost Averaging |
| Debt     | Loan / Mortgage, Credit Card Payoff |
| Planning | Retirement, Inflation, Investment Return, Net Present Value |
| Business | Break-even, ROI |

## Usage

Just open `index.html` in any browser. That's it.

```bash
git clone https://github.com/AgentColonyAI/calcstack
open calcstack/index.html
```

No npm install. No server. No accounts.

## Deploy to GitHub Pages (free)

1. Fork this repo
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch → main → / (root)**
4. Your app is live at `https://agentcolonyai.github.io/calcstack/`

## Deploy to Netlify (free, one click)

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/AgentColonyAI/calcstack)

Or drag-and-drop `index.html` into [netlify.com/drop](https://app.netlify.com/drop).

## Deploy to Vercel (free)

```bash
npm i -g vercel
vercel --yes
```

## Features

- **Zero dependencies** at runtime (Chart.js loaded from CDN)
- **Dark mode** toggle built in
- **Responsive** — sidebar collapses on mobile
- **All math runs locally** — no API calls, no tracking, no ads
- Single `index.html` — easy to self-host, fork, or embed

## Contributing

PRs welcome. Each calculator is a self-contained section in `index.html` — easy to find and modify.

To add a calculator:
1. Add a nav item in the sidebar with `data-calc="yourname"`
2. Add a `<section class="calc-section" id="calc-yourname">` in the content area
3. Add a `calcYourname()` function in the script
4. Register it in the `calcFns` object at the bottom

## License

MIT — use it, fork it, ship it.
