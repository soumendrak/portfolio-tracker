<div align="center">

<img src="./logo.svg" alt="Portfolio Tracker v2" width="120" />

# Portfolio Tracker v2

**Track your investments, dividends, and financial goals — all in your browser.**

[![License: MIT](https://img.shields.io/badge/license-MIT-blue?style=flat)](./LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)]()
[![Vanilla JS](https://img.shields.io/badge/Vanilla-JS-F7DF1E?style=flat&logo=javascript&logoColor=black)]()
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat)]()

</div>

---

## Overview

**Portfolio Tracker v2** is a single-file HTML web app for tracking your stock portfolio. No frameworks, no CDN dependencies, no signups. Everything runs in your browser with localStorage persistence.

Built for the modern investor who wants a clean, dark-themed dashboard to monitor holdings, dividends, and progress toward financial goals.

## Features

| Feature | Description |
|---|---|
| **Portfolio Dashboard** | Total value, P&L, return %, annual dividend income at a glance |
| **Holdings Table** | Add/edit/remove stocks with ticker, shares, buy price, current price |
| **Allocation Pie Chart** | SVG pie chart showing portfolio allocation by holding |
| **Dividend Calendar** | Monthly calendar view of expected dividend payouts |
| **Goal Tracking** | Visual progress bars for income (Rs 2.5L/mo) and corpus (Rs 10Cr by 2029) targets |
| **yfinance Proxy** | Optional: fetch live prices via a Cloudflare Worker proxy |
| **Import/Export** | Backup and restore your portfolio as JSON |
| **Zero Dependencies** | Single index.html — no npm, no CDN, no build step |

## Quick Start

```bash
# Clone the repo
git clone https://github.com/soumendrak/portfolio-tracker.git
cd portfolio-tracker

# Open in browser
open index.html
# Or serve with any static server:
python3 -m http.server 8080
```

## Screenshot

![Portfolio Tracker Screenshot](./screenshot.png)

## Project Structure

```
portfolio-tracker/
  index.html    — The entire application
  LICENSE       — MIT License
  README.md     — This file
  logo.svg      — Project logo
```

## Architecture

- **Vanilla JS** — No frameworks. DOM manipulation via native APIs.
- **localStorage** — All data stored client-side. No server needed.
- **SVG Charts** — Pie chart rendered with SVG `<path>` arcs.
- **CSS Custom Properties** — Dark theme via `:root` variables for easy customization.
- **yfinance Proxy Pattern** — Optional Cloudflare Worker endpoint for live prices. Falls back to manual entry.

## License

MIT — see [LICENSE](./LICENSE)
