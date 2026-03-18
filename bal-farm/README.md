# 🥚 Bal Farm — Egg Harvest Tracker

A simple, offline-capable web app for tracking daily egg harvests on your poultry farm. Built for Philippine peso (₱) farms.

## Features

- **Daily Egg Logging** — Log Small, Medium, Large, Jumbo, and Broken eggs
- **Live Calculations** — See income per size and total income as you type
- **Laying Rate** — Automatic % calculation based on your flock size
- **History** — Filter by Today, Last 7 Days, Last 30 Days, or custom date range
- **Reports** — Weekly & monthly charts, breakdowns, and summaries
- **Editable Prices** — Set your own price per egg size (defaults: ₱5/6/7/8)
- **Flock Management** — Track your total chicken count
- **Offline-ready** — No backend needed, all data stored in your browser (localStorage)
- **Mobile-friendly** — Works on phones and tablets

## Screenshots

> Live at: `https://<your-github-username>.github.io/bal-farm`

## How to Use

### Option 1 — Use directly on GitHub Pages (recommended)
1. Fork or push this repo to your GitHub account
2. Go to **Settings → Pages → Source: GitHub Actions**
3. The app will deploy automatically to `https://<username>.github.io/bal-farm`

### Option 2 — Run locally
Just open `index.html` in any modern browser. No install needed.

## Deploying to GitHub Pages (step by step)

1. Create a new GitHub repository named `bal-farm`
2. Upload all files (or push via git):
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/<your-username>/bal-farm.git
   git push -u origin main
   ```
3. Go to your repo on GitHub → **Settings** → **Pages**
4. Under **Build and deployment**, set Source to **GitHub Actions**
5. The workflow in `.github/workflows/deploy.yml` will auto-deploy on every push
6. Your app will be live at `https://<your-username>.github.io/bal-farm`

## Data Storage

All data is saved in your browser's **localStorage** under these keys:
- `balFarm_logs` — harvest records
- `balFarm_prices` — egg prices per size
- `balFarm_flock` — chicken count

> ⚠️ Clearing browser data will delete your farm records. For backup, use your browser's export tools or copy the localStorage values.

## Tech Stack

- Pure HTML + CSS + Vanilla JavaScript
- No frameworks, no dependencies, no build step
- Google Fonts (Lora + DM Sans) loaded from CDN

## License

MIT — free to use and modify.
