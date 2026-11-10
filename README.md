# Trade Calendar Journal

Responsive trading journal for GitHub Pages. No build step or external libraries.

## Deploy
Upload `index.html` to your GitHub repository, commit/push, then enable GitHub Pages under **Settings → Pages**.

## Features
- Week / Month / Year / All-time views
- Monthly calendar with daily net P&L and trade count
- Add, edit and delete trades
- Long and Short P&L calculated from entry, exit, quantity and fees
- Net P&L, win rate, wins/losses, breakeven, profit factor, average win/loss, best/worst trade
- Monthly P&L goal and daily P&L chart
- JSON Backup / Restore
- Mobile responsive layout

## P&L formula
Long: `(Exit - Entry) × Quantity - Fees`
Short: `(Entry - Exit) × Quantity - Fees`

Quantity means base-asset / contract units matching the quote currency. For derivatives, check your exchange's contract specification. Include funding/borrow charges manually in Total fees if you want them included.

## Data storage
Trades are stored in this browser's LocalStorage. Refreshes and browser restarts keep data, but it does not sync across devices/browsers. Clearing site data, using private mode, or resetting/uninstalling the browser may erase it. Download JSON backups regularly. Restore replaces the current local journal with the backup.

This is a journal, not a broker connection or financial advice.
