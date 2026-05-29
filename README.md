# Mama's Bakcang — Order Dashboard

A simple, offline-ready business dashboard for managing home food orders.

## Features
- Add and track orders (Bakcang, Pineapple Tart, etc.)
- Track order status: New → Preparing → Ready → Delivered
- Delivery view with customer address & phone
- Payment tracking (paid / unpaid)
- Revenue summary by product and top customers

## Tech
Pure HTML + CSS + JavaScript. No framework, no build step. Data is stored in `localStorage` (browser storage — stays on the device).

## Deploy to Vercel

### Option 1 — Vercel CLI
```bash
npm install -g vercel
vercel
```

### Option 2 — Vercel Dashboard
1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project
3. Import your GitHub repo
4. Leave all settings as default → click Deploy

That's it. Vercel auto-detects it as a static site.

## Run locally
Just open `index.html` in your browser. No server needed.

## Notes
- Data is stored in the browser's localStorage. It won't sync between devices.
- To back up data: open browser console and run `JSON.stringify(localStorage.getItem('bakcang_orders_v1'))` and save the output.
