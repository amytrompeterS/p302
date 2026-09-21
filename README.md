# Atelier North — Buyer Intelligence Dashboard

A merchandising dashboard for the Chicago location of a national bridal boutique chain. Designed to help buyers monitor sales performance, identify top and slow-moving gowns, and make data-informed purchasing decisions.

---

## Features

- **KPI summary cards** — Overall sales, seasonal sales, promo lift, and inventory turn with month-over-month change indicators
- **Sales charts** — Monthly bar chart and seasonal trend line with promo lift overlay
- **Best sellers & slow movers** — The top 5 and bottom 5 dresses ranked by sales volume, with SKU, silhouette, fabric, price, and trend
- **Buyer recommendations** — Insights from peer store performance to guide future buying strategy
- **Month filter** — App bar picker filters all cards and charts to a single month or the full year

---

## Tech Stack

| Layer | Library |
|---|---|
| Framework | Vue 3 + `<script setup>` |
| Language | TypeScript |
| UI components | Vuetify 4 |
| Charts | Chart.js via vue-chartjs |
| Build tool | Vite |
| Icons | Material Design Icons (`@mdi/font`) |

---

## Getting Started

**Prerequisites:** Node.js 18+

```bash
# Install dependencies
npm install

# Start the dev server
npm run dev
```

The app runs at **http://localhost:5173** by default.

```bash
# Type-check and build for production
npm run build

# Preview the production build locally
npm run preview
```

---

## Project Structure

```
src/
├── data/
│   └── metrics.json       # 12-month sales dataset (Jan–Dec 2025)
├── views/
│   └── HomeView.vue       # Main dashboard — all logic and layout
├── plugins/
│   └── vuetify.ts         # Vuetify configuration
├── router/
│   └── index.ts           # Vue Router setup
└── main.ts                # App entry point
```

---

## Data

`src/data/metrics.json` contains simulated data for 12 months (Jan–Dec 2025). Each month includes:

- **Sales by SKU** — revenue per dress across 10 SKUs (`BR-1042` through `BR-1931`)
- **Seasonal sales** — overall store seasonal revenue
- **Promo lift** — percentage uplift attributed to promotions
- **Inventory turn** — annualized inventory turnover rate

All figures trend upward across the year with realistic month-to-month variation.

---

## Design

- Light theme with a neutral palette and teal/blue accents
- Clean, minimal layout with generous whitespace
- Fully responsive — cards and sections stack on mobile
