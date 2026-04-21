# Trading Bot

Autonomous swing trading agent built on Claude Code cloud routines + Alpaca.

## Quick start (local)

```bash
cp env.template .env
# Fill in credentials
# Open repo in Claude Code, then:
/portfolio   # smoke test — should print account + positions
```

## Structure

| Path | Purpose |
|------|---------|
| `CLAUDE.md` | Agent rulebook, auto-loaded every session |
| `scripts/` | API wrappers (Alpaca, Perplexity, ClickUp) |
| `routines/` | Cloud routine prompts — paste verbatim into the web UI |
| `.claude/commands/` | Local slash commands for manual runs |
| `memory/` | Persistent state committed to main |

## Cron schedule (America/Chicago, weekdays)

| Routine | Cron | Time |
|---------|------|------|
| pre-market | `0 6 * * 1-5` | 6:00 AM |
| market-open | `30 8 * * 1-5` | 8:30 AM |
| midday | `0 12 * * 1-5` | 12:00 PM |
| daily-summary | `0 15 * * 1-5` | 3:00 PM |
| weekly-review | `0 16 * * 5` | 4:00 PM Fridays |

## Setup checklist

- [ ] Install Claude GitHub App on this repo
- [ ] Create 5 cloud routines (see `routines/` + Part 7 of setup guide)
- [ ] Set env vars on each routine (never commit `.env`)
- [ ] Enable "Allow unrestricted branch pushes" on each routine
- [ ] Local smoke test: `/portfolio` prints cleanly
- [ ] Seed TRADE-LOG.md with Day 0 baseline before first live run
