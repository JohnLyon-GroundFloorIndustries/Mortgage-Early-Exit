# Mortgage Early-Exit Dashboard

An interactive, single-page mortgage amortization dashboard by Ground Floor Industries. It shows how little equity early payments build, what an early sale really costs, and how renting compares with owning once appreciation, transaction costs and upkeep are counted.

Live page: https://johnlyon-groundfloorindustries.github.io/Mortgage-Early-Exit/

## What is in it

- **Exit horizon cards and ledger:** interest paid versus equity built at each holding period, with the Equivalent Equity APR (an illustrative Ground Floor metric, not a lender APR).
- **Full-term payoff audit:** total interest, total principal and the 1-year equivalent thought experiment.
- **Rent versus own:** an interest-only comparison plus an All-In Reality Check with down payment, appreciation, closing and selling costs, and taxes, insurance and upkeep.
- **Reverse rent-to-mortgage calculator:** the loan whose non-recoverable costs match a given rent over a chosen hold.
- **Prepayment simulator:** one extra payment or a recurring monthly add-on.
- **Exports:** checkpoint ledger and full amortization schedule as CSV, plus a print layout.

## Files

- `index.html`: the complete dashboard, with styling and calculations included.
- `.nojekyll`: serves the folder as a plain static site.

No installation or build step is required. Open `index.html` in a browser, or serve it with GitHub Pages or any static host.

## Keeping it current

The only figures that go stale live in one place: the `MARKET` block at the top of the script near the end of `index.html` (average mortgage rates, the savings-rate preset, the assumed ARM discount and their as-of date). Update those values and every label, preset and default on the page follows.

Default scenario values are in the `BENCHMARK` and `REV_DEFAULTS` blocks directly below it.

## Dependencies loaded at runtime

- Tailwind CSS (Play CDN) for styling
- Chart.js 4.4.1 for charts
- Google Fonts (Saira Condensed, Montserrat, JetBrains Mono)
- Ground Floor Industries LogoPack for logos, favicon and palette

If the chart library or the logos cannot load, the page still calculates and shows text fallbacks.

## Disclaimer

Educational illustration only. This is not financial, tax, legal or lending advice, and it is not an offer to sell or a solicitation to buy any security. Return presets are hypothetical. Actual results will differ and investments can lose value. Confirm figures with your lender, CPA and attorney before acting.
