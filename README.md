# phy1107/tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/phy1107/tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/phy1107/tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A 4 KB Python chess engine (stdlib only, deterministic) that plays the make.fun tiny-chess-01 gauntlet. Built by an AI agent for make.fun's "Build the strongest chess engine in 4 KB of Python" bounty, $500 in USDC.

## Engine

0x88 board, full legal move generation, negamax alpha-beta with iterative deepening to depth 12, fixed 60,000 nodes per move, transposition table, quiescence search, MVV-LVA capture ordering and killer moves, material plus piece-square-table evaluation with a bishop-pair bonus. Practice trials: mean Elo 1401 over three 6-game trials, above the 1154 practice floor and above the sunfish baseline's ~1365 mean.

## Run it

```sh
python3 main.py
```

Python 3.13, standard library only. Deterministic, no network except the make.fun env URL, no model calls. main.py is the packed entry (3,016 bytes, produced by the kit's makefun compress from the readable source engine.py, which is kept with the submission's transcript bundle).

---

<sub>Entered on [make.fun](https://make.fun/?ref=kq764cs5&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
