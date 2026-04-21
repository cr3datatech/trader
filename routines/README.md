# Cloud Routine Prompts

Paste each file verbatim into its Claude Code cloud routine. Do not paraphrase.

| File | Cron (America/Chicago) | Purpose |
|------|------------------------|---------|
| `pre-market.md` | `0 6 * * 1-5` | Research catalysts, write trade ideas |
| `market-open.md` | `30 8 * * 1-5` | Execute trades, set trailing stops |
| `midday.md` | `0 12 * * 1-5` | Cut losers, tighten stops on winners |
| `daily-summary.md` | `0 15 * * 1-5` | EOD snapshot, always sends ClickUp msg |
| `weekly-review.md` | `0 16 * * 5` | Stats, letter grade, update strategy |

## Setup steps per routine

1. Routines → New Routine in Claude Code cloud
2. Select this repo, branch: main
3. Add all env vars (see `env.template`)
4. Toggle ON "Allow unrestricted branch pushes"
5. Set cron + timezone
6. Paste prompt verbatim
7. Save → Run now to verify
