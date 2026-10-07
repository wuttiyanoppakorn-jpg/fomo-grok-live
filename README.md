# FOMO x GROK — paper trading dashboard

Live page: https://wuttiyanoppakorn-jpg.github.io/fomo-grok-live/

**MODE: PAPER — simulated trades only, no real money.**

A copy-trading bot follows 9 traders on fomo.family and records *paper* buys/sells here.
- `ledger.json` — open positions, closed trades, last run (updated automatically by the bot's 5-minute routine)
- `config.json` — rules: $5 flat per buy, take-profit / stop-loss from entry, 1% fee/slippage each side assumed
- `index.html` — dashboard; re-reads the JSON every 30s and polls DexScreener for live display prices

Live prices on the page are display-only; authoritative TP/SL exits are decided by the bot's routine.
