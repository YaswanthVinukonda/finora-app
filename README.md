# FINORA — Personal Finance

A local-first, installable personal finance tracker.

## Features
- Income, expense and investment entries
- Multi-currency transaction recording
- Wallets and account balances
- Monthly budgets and spending categories
- Assets, liabilities and net-worth overview
- CSV export and JSON backup/restore
- Local browser storage; no bank connection or cloud database
- Installable PWA shell with offline caching

## Deploy
GitHub Actions deploys this repository to GitHub Pages on every push to `main`.

After the first successful deployment:
1. Open the GitHub Pages URL in Safari on iPhone.
2. Tap Share → Add to Home Screen → Add.
3. Launch FINORA from the home screen.

## Data safety
Financial records are stored in the browser's local storage for this website origin. Export JSON backups regularly. Clearing Safari website data, changing browsers/devices, or changing the website origin can make existing local records unavailable. The service worker caches the app shell only; it does not back up transaction data.

## Currency handling
Transactions retain their original currency. Live foreign-exchange rates and automatic cross-currency consolidation are not implemented yet.
