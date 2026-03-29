# Video Game Sales Dashboard

Interactive dashboard analyzing global video game sales from 1980 to 2017.
Covers 16,326 titles across 31 platforms, 12 genres, and 576 publishers,
with a total of 8.82 billion units sold worldwide.

## Dataset

Source: Video Game Sales Dataset (Kaggle)
Format: XLSX with 16,326 records and 10 variables.
Includes game title, platform, release year, genre, publisher,
and sales figures broken down by North America, Europe, Japan, Rest of World, and Global.
Public dataset available at: https://www.kaggle.com/datasets/gregorut/videogamesales

## Tools

- HTML5 + CSS3 — layout, animations, scanline overlay, glitch effects and neon glow styling
- Chart.js 4.4.0 — bar, line, doughnut, polar area and stacked charts (9 chart types used)
- Google Fonts — Orbitron (headings) and Share Tech Mono (data/body)
- Vanilla JavaScript — tab navigation, lazy chart initialization, heatmap rendering and live clock
- GitHub Pages — static deployment, no backend required

## Dashboard Sections

Five fully independent tabs, each with dedicated charts, KPI cards and data tables:

**Overview** — 6 KPI cards (total titles, global sales, #1 game, peak year, top publisher, top genre), top 20 best-selling games, regional breakdown with stat cards, top 15 platforms, genre polar area chart, annual sales timeline, top 10 publishers with proportional bars, genre×region grouped comparison, publisher market share donut, platform stacked regional split, top 25 games full intel table with mini-bars, yearly sales heatmap (1983–2016) and title count per platform.

**Platforms** — 5 KPIs (best-selling platform, most titles, Gen 7 winner, top handheld, total platforms), top 15 platforms horizontal bar, console generation comparison (Gen 3 through Gen 8 + handheld), regional stacked breakdown for 12 platforms, title count chart and a detailed table with maker, era, total sales, game count and top game per platform.

**Publishers** — 5 KPIs, top 15 publishers horizontal bar, regional breakdown (NA/EU/JP/Other) for top 8 publishers, genre composition per publisher (stacked bar across 6 genres), market share donut and full table with per-region split for 15 publishers.

**Regions** — 4 large territory cards (NA 49.2%, EU 27.3%, JP 14.5%, Other 9.0%) each showing top game, top genre and top platform, regional sales timeline with 4 lines from 1995–2016, genre preference by region, platform dominance by region and four individual genre-composition donuts per territory.

**Timeline** — 5 era summary cards (Dawn 1980–89, Growth 1990–99, Golden 2000–07, Peak 2008–11, Consolidation 2012–16), full 1980–2016 combo bar+line chart, genre evolution across five-year buckets, console manufacturer stacked area (Nintendo/Sony/Microsoft/Sega/Others) and a year-by-year records table with YoY% change and best-selling game per year.

## Visual Style

Cyberpunk 2077 aesthetic built entirely in CSS: neon yellow (#FFE000), cyan (#00F5FF) and magenta pink (#FF0090) accents over a near-black deep purple background (#03020A). Full-viewport scanline overlay via repeating-linear-gradient, subtle perspective grid in the background, and a glitch animation on the main title using layered ::before/::after pseudo-elements with clipped pink and cyan ghost copies. KPI cards and panels use angled clip-path corners with colored top-border glow. Navigation tabs light up with neon glow on the active state. An animated ticker scrolls key metrics horizontally across the header. All interactive elements respond with border and background hover transitions. Pulse dot indicator animates on the live system clock in the footer.

Fully client-side — no backend, no build step, no frameworks. Single index.html file. Only external dependency is Chart.js 4.4.0 via CDN.

## Live Demo

[View Dashboard](https://painkiller-gh.github.io/videogame-sales-dashboard/)
