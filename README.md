# linerup-record — public, tamper-evident record

Immutable, timestamped record of every linerup.bet prediction.

Going forward, each day's slate is committed here **before first pitch**. GitHub
timestamps every commit and the history is append-only, so anyone can verify a
pick existed before the game started and that no result was altered or deleted
afterward.

- `mlb/snapshot-YYYY-MM-DD.json` — MLB slate published that day
- `nba/snapshot-YYYY-MM-DD.json` — NBA slate published that day

The first commit is a one-time backfill of prior snapshots (imported on the commit
date, not pre-game proof). Every commit after it is the live, pre-game record.

Live: https://linerup.bet · Track record: https://linerup.bet/track-record
