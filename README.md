# The Corner Café dashboard

A browser-based prototype of a café dashboard for quickly checking daily performance, reviewing menu-item sales, and monitoring stock. It is intended for user testing; all figures are fictional sample data, not live business information.

## Features

- **Overview:** today's sales and order totals, busiest hour, an hourly orders chart, and a stock-reorder summary.
- **Sales by item:** compare items sold yesterday or over the last seven days; sort by units sold, revenue, or name.
- **Item details:** view an item's price, category, stock status, seven-day sales totals, and daily sales.
- **Stock levels:** search menu items, optionally filter to items that need reordering, and see stock quantities and reorder thresholds.
- **Responsive, accessible navigation:** hash-based screens support browser Back/Forward, with a collapsible mobile menu, keyboard focus handling, and screen-reader status updates.

Some controls—such as Settings, report downloads, spreadsheet export, editing items, and reordering—are placeholders. They open a message explaining that the functionality is not part of this prototype.

## Run locally

No build step or package installation is required. Open `index.html` in a modern web browser. The page loads Bulma CSS from jsDelivr, so an internet connection is needed for the stylesheet.

## Data and implementation

The app is implemented in a single HTML file with inline CSS and JavaScript. Menu items, stock quantities, sales, and order counts are generated or defined in the page and kept in memory; there is no backend, persistence, or connection to a point-of-sale system. The seeded sales data is repeatable when the page is reloaded.
