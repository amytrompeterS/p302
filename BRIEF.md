# Retail Data Story 302- Project Brief

## What is this?
A buyer at the Chicago location of a national bridal dress shop chain needs a dashboard to monitor business operations and product sales to impact their future buying strategies.

## Data
Generate a fake dataset as a JSON file (src/data/metrics.json). 
12 months of data (Jan-Dec 2025), each month containing:
- Sales by SKU (amount, trending upward with some variation)
- Seasonal sales patterns (amount, trending upward with some variation)
- Promo Lift (percentage, trending upward with some variation)
- Inventory Turn (amount, trending upward with some variation)

## Layout (Vuetify)
- v-app-bar at the top with the dashboard title and a month picker
- the month picker should default to showing ALL months
- When a specific month is select, all cards and charts filter to that month. When "All" is selected, show the full year
- Below the app bar: a row of 4 summary cards (v-cards) showing the key metrics: Overall sales, seasonal sales, promo lift, inventory turn
- Below that: one half-width section with best the 5 best-selling dresses. For each item include sku number, sales volume, trend in sales, image of dress, style of dress (examples: Ballgown, mermaid, trumpet, A-line), fabric, price per sku
- Next to that: one half-width section with the 5 worst-selling dresses. For each item include sku number, sales volume, trend in sales, image of dress, style of dress (examples: Ballgown, mermaid, trumpet, A-line), fabric, price per sku
- Below that: include a recommendations section. Include specific dresses, dress styles and fabrics that are selling well at other store locations
- use v-container, v-row, v-col for responsive grid layout

## Interactions
- Month picker in the app bar filters EVERYTHING - summary cards show that month's number, charts highlight or filter to that month
- When "ALL" is selected, summary cards show yearly totals/averages and charts show all 12 months
- Cards show a small up/down arrow or color indicating change from the previous month

## Style
- light theme by default 
- clean, minimal, lots of whitespace, sophisticated design
- charts should use a cohesive color palette of neutrals with accents of light blue - not rainbow
- mobile responsive - cards stack on small screens

## Tech
- Vue 3 + TypeScript + Vuetify 3