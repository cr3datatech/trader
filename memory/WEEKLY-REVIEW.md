# Weekly Review

Friday reviews appended here.

Template for each entry:

## Week ending YYYY-MM-DD

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $X |
| Ending portfolio | $X |
| Week return | ±$X (±X%) |
| S&P 500 week | ±X% |
| Bot vs S&P | ±X% |
| Trades | N (W:X / L:Y / open:Z) |
| Win rate | X% |
| Best trade | SYM +X% |
| Worst trade | SYM -X% |
| Profit factor | X.XX |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |

### What Worked
- ...

### What Didn't Work
- ...

### Key Lessons
- ...

### Adjustments for Next Week
- ...

### Overall Grade: X

---

## Week ending 2026-04-24

### Stats
| Metric | Value |
|--------|-------|
| Starting portfolio | $100,000.00 (Day 0 baseline) |
| Ending portfolio | $100,000.00 (API unreachable — confirmed all-cash from log) |
| Week return | $0 (0.00%) |
| S&P 500 week | ~+1.1% est (ES Mon open ~7,064 → Fri close ~7,108–7,142; Perplexity unavailable) |
| Bot vs S&P | ~-1.1% est |
| Trades | 0 (W:0 / L:0 / open:0) |
| Win rate | N/A |
| Best trade | N/A |
| Worst trade | N/A |
| Profit factor | N/A |

### Closed Trades
| Ticker | Entry | Exit | P&L | Notes |
|--------|-------|------|-----|-------|
| — | — | — | — | No trades executed — Alpaca proxy unreachable all week |

### Open Positions at Week End
| Ticker | Entry | Close | Unrealized | Stop |
|--------|-------|-------|------------|------|
| — | — | — | — | — |

### What Worked
- Patience discipline: HOLD every day was correct given VIX 19–19.5 and binary Iran/Hormuz ceasefire risk
- Research quality strong: correctly identified TXN (+19% post-earnings), NOC record backlog, SLB Hormuz tailwind — all confirmed in price action
- PDT capacity preserved (0/3 used) — full flexibility entering next week
- Sector mapping accurate: Energy + Defense + Materials leading; Tech/Consumer Dis lagging
- TXN non-chase decision proved correct — +19% gap would have been dangerous entry point

### What Didn't Work
- Alpaca proxy (178.104.75.110:8080) unreachable every session — 10 consecutive failures; zero trades executable
- PERPLEXITY_API_KEY, CLICKUP_API_KEY, CLICKUP_WORKSPACE_ID, CLICKUP_CHANNEL_ID all missing — no S&P benchmarking, no notifications all week
- Bot launched with broken infrastructure — should have been smoke-tested before go-live
- Zero capital deployed all week (0% vs target 75–85%) — complete operational failure
- No real GTC stops placed because no positions to protect

### Key Lessons
- Infrastructure must be verified (proxy + all env vars) before bot launch — not during
- Missing even one critical env var cascades to silent workflow failures across all steps
- Good research + correct strategy = irrelevant when API is down; resolve connectivity first
- S&P returned ~+1% while bot sat 100% cash — first week already underwater vs benchmark
- TXN, NOC, SLB remain valid watchlist candidates for week 2 entry if API is restored

### Adjustments for Next Week
- CRITICAL: Resolve Alpaca proxy connectivity before Monday open — no bot run until confirmed
- CRITICAL: Inject all env vars (PERPLEXITY_API_KEY, CLICKUP_API_KEY, CLICKUP_WORKSPACE_ID, CLICKUP_CHANNEL_ID) before Monday
- Entry targets for week 2 (if API live): TXN pullback $225–235, NOC $490–500, SLB post-earnings $47–49
- VIX watch: still elevated ~19; size ≤15% per position until VIX < 17
- Weekly trade budget: 0/3 used — full 3-trade capacity available
- Brent $105 + Hormuz: Energy/Defense sectors remain in momentum; favor these over Tech

### Overall Grade: D+
*Strategy discipline: A. Research quality: B+. Infrastructure: F. Net result: D+ — correct process, broken tooling, zero execution.*
