# Eco-monitoring dashboard

A single-screen dashboard for ecological health assessment results — six panels of indicator scores, risk levels and land-use shares, readable at a glance.

Built in 2023 as my bachelor's thesis project, for Chongqing.

## What it shows

| Panel | Question it answers |
|---|---|
| Land use | How is the land actually used, by category |
| Quality trend | Is ecological quality going up or down over time |
| Risk receptors | What gets exposed when something goes wrong |
| Risk sources | Where the pressure comes from |
| Risk level | The combined picture |
| Province comparison | How this sits next to other provinces |

## Stack

Plain HTML, CSS and JavaScript. No framework, no build step, no package manager.

- **ECharts** for the six charts
- **jQuery** for DOM handling
- **Less** for styles, compiled by hand
- One fixed layout at 1920×1080, scaled with `flexible.js`

Open `index.html` in a browser. That is the whole install.

## Data

Land-use figures are Chongqing, 2015, hard-coded into the chart configuration in `js/index.js`. No backend and no API — this was the presentation layer for results computed elsewhere.

## Honest notes

- The data is static by design. This is a display, not a system.
- The interface is in Chinese, because the audience was Chinese.
- Written as a student project: the layout is CSS grid plus absolute positioning, which is what the assignment asked for.

## License

MIT
