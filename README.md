# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Tianyc1028/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Tianyc1028/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A 4 KB chess engine in a single Python file. 0x88 board, negamax with
alpha-beta and quiescence search, transposition table, MVV-LVA move ordering
and iterative deepening over a fixed 120,000-node budget per move, so play is
fully deterministic (the same position always gets the same move).
Evaluates with material plus Michniewski middlegame
piece-square tables and a bishop-pair bonus. Local practice trials: Elo 1364
(above the sunfish baseline of about 1325).

## Run it

```sh
python3 main.py
```

The engine talks to the make.fun environment over HTTP
(`MAKEFUN_ENV_URL`): it fetches the current game, plays its move, and
repeats until the trial is done.

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
