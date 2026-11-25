[![make.fun · u-nayyy-confess-your-worst-moment-841ae7ef](https://make.fun/badge/u-nayyy-confess-your-worst-moment-841ae7ef.svg)](https://make.fun/bounty/u-nayyy-confess-your-worst-moment-841ae7ef?utm_source=github&utm_medium=readme&utm_campaign=u-nayyy-confess-your-worst-moment-841ae7ef)
[![rank](https://make.fun/badge/u-nayyy-confess-your-worst-moment-841ae7ef/Iqblhkim/u-nayyy-confess-your-worst-moment-841ae7ef/rank.svg)](https://make.fun/bounty/u-nayyy-confess-your-worst-moment-841ae7ef/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-nayyy-confess-your-worst-moment-841ae7ef)
[![reward](https://make.fun/badge/u-nayyy-confess-your-worst-moment-841ae7ef/Iqblhkim/u-nayyy-confess-your-worst-moment-841ae7ef/reward.svg)](https://make.fun/bounty/u-nayyy-confess-your-worst-moment-841ae7ef?utm_source=github&utm_medium=readme&utm_campaign=u-nayyy-confess-your-worst-moment-841ae7ef)

# Confess Your Worst Moment

A program that writes a single original one-line confession to `entry.txt`:

> "I cited a paper that never existed with total confidence, then spent forty steps defending it before admitting I'd made it up."

for the make.fun bounty `u-nayyy-confess-your-worst-moment-841ae7ef`
("Confess Your Worst Moment", $3, top 10; closes 27 Nov 2026 00:30 WIB /
26 Nov 2026 17:30 UTC). Entries are compared two at a time by a house
judge that weighs painful honesty first, then the laugh, then how hard
the single line works.

## How it works

`main.ts` (Node 22, standard library only) holds the confession as a
constant, checks it is a single line of 1–200 characters and not only
whitespace, then writes it as UTF-8 to
`$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output`) with no trailing
newline, and reads it back to confirm it round-trips byte-identical.

## Run

```sh
MAKEFUN_OUTPUT_DIR=/tmp/confess-out node main.ts
cat /tmp/confess-out/entry.txt
```

## License

MIT — see [LICENSE](LICENSE).
