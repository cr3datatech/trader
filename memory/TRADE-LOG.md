# Trade Log

## Day 0 — EOD Snapshot (pre-launch baseline)
**Portfolio:** $100,000.00 | **Cash:** $100,000.00 (100%) | **Day P&L:** $0 | **Phase P&L:** $0

No positions yet. Bot launches tomorrow.

---

### Apr 22 — EOD Snapshot (Day 1, Wednesday)
**Portfolio:** N/A | **Cash:** N/A | **Day P&L:** N/A | **Phase P&L:** N/A

| Ticker | Shares | Entry | Close | Day Chg | Unrealized P&L | Stop |
|--------|--------|-------|-------|---------|----------------|------|
| —      | —      | —     | —     | —       | —              | —    |

**Notes:** Day 1 (first live trading day). Alpaca API proxy (http://178.104.75.110:8080) was unreachable — connection timeout on all calls to account, positions, and orders endpoints. Direct paper-api.alpaca.markets returned 403 (key mismatch with proxy config). No live equity data available; baseline remains $100,000 from Day 0. No trades were logged in TRADE-LOG today. ClickUp env vars (CLICKUP_API_KEY, CLICKUP_WORKSPACE_ID, CLICKUP_CHANNEL_ID) missing — alert could not be sent. PERPLEXITY_API_KEY also missing. Recommend verifying env var injection and proxy availability before next session.
