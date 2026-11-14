# Muse Spaces — F&B Sales Dashboard (Acme Cafe demo)

A sales dashboard for F&B owners, built with Muse. This repo holds the Acme Cafe demo: synthetic data only, not real sales.

Live demo: https://fnb.courseoss.com/ (also https://muse-spaces-fnb-sales-ga4.tembusu.workers.dev/)

## What is in this repo

- `index.html` — the Acme Cafe Sales Dashboard demo (October 2026, Demo — Synthetic). Sales today and this month, best seller, daily sales chart, sales by dish, sales timing, daily takings by payment type with day / month / year filters, sales bridge, variance table, inventory level, cost of sales, expenses, website & reviews, 3 key drivers, reminders, and a reconciliation line. GA4 pageview tracking is included via the gtag snippet in the page head.
- `Muse_for_F_B___Sales_Dashboard_Setup_v7.md` — the setup prompt (v7). Part 1 is the tap-to-approve interview prompt that builds *your* dashboard in one Muse chat. Part 2 is the replica PRD (features, layout order, exact numbers, style tokens, verification protocol). Part 3 is the implementation prompt for rebuilding the dashboard one-to-one from the PRD and the mock.
- `wrangler.jsonc` — Cloudflare Worker config for static hosting.

## Use it

1. Open `index.html` to see what "done" looks like (Acme Cafe, Demo — Synthetic).
2. To build your own dashboard, attach `Muse_for_F_B___Sales_Dashboard_Setup_v7.md` to a new Muse chat and tap **Start setup**. Muse asks one question at a time, with Skip / Pending every time.
3. To rebuild this demo one-to-one, attach the v7 file and `index.html` to a new Muse chat and paste the Part 3 implementation prompt. The PRD in Part 2 is the source of truth; the verification protocol in it checks the rebuild section by section until the diff log is empty.

## Data

All figures are Demo — Synthetic (13,781 synthetic sales, 1 Jan 2025 – 9 Nov 2026). Demo and real sales are never mixed. No personal data, no real takings.

## Deploy

```sh
npx wrangler deploy
```

## Buy the setup prompt

Muse for F&B — Sales Dashboard Setup: https://buymeacoffee.com/bencheng/e/596578
