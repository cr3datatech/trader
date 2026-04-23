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

---

### Apr 23 — Market-Open (Day 2, Thursday)
**Portfolio:** N/A | **Cash:** N/A (API unreachable — 4th consecutive session)

| Ticker | Shares | Entry | Fill | Stop | Thesis | Target | R:R |
|--------|--------|-------|------|------|--------|--------|-----|
| —      | —      | —     | —    | —    | —      | —      |  — |

**Notes:** Market-open execution attempted. Alpaca proxy (http://178.104.75.110:8080) still unreachable (timeout, exit 124). Direct paper-api.alpaca.markets returns 403 — API key is bound to proxy. No trades executable. Research log for today already complete (pre-market run); watchlist: INTC post-earnings, LMT post-earnings, CVX/XOM on pullback. Weekly trade count: 0/3. No ClickUp notification (keys missing). CRITICAL: resolve proxy connectivity and env var injection before session 5.

### Apr 23 — Midday Scan (Day 2, Thursday)
**Portfolio:** N/A | **Cash:** N/A (API unreachable — 5th consecutive session)

- Alpaca proxy (http://178.104.75.110:8080) timeout on both `positions` and `orders` calls (exit 28).
- No open positions confirmed from log history → Steps 3/4/5 (cut losers, tighten stops, thesis check) all N/A.
- PERPLEXITY_API_KEY, CLICKUP_API_KEY, CLICKUP_WORKSPACE_ID, CLICKUP_CHANNEL_ID all MISSING — Steps 6/7 skipped.
- No action taken. All cash. Watchlist unchanged: INTC, LMT, CVX/XOM.
- CRITICAL: proxy and env var injection still broken — 5 sessions with zero trades executable.
