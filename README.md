# UniPredict

Orange and black prediction market on Sphere testnet (UCT). Static site, no build step.

## Deploy from a phone
1. On github.com create a new repository, then upload `index.html`, `markets.json` and `README.md`.
2. On vercel.com sign in with GitHub, tap Add New, then Project, and import the repository.
3. Leave all settings empty (Framework: Other) and tap Deploy.

## Setup
In `index.html` change `escrow` in CONFIG to your Sphere nametag or address. This is where stakes are sent.

## Add a market (dev only)
Open `markets.json` on GitHub, tap the pencil icon, copy an existing market block, change the fields and commit. Vercel redeploys automatically. Only people with write access to the repo can add markets.

- `timeframe`: daily, weekly or monthly
- `category`: crypto, esports or politics
- `ends`: UTC time. After this moment the pool closes and betting is disabled.
- `outcome`: add `"yes"` or `"no"` to settle a market.
