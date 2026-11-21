# tiny-chess-gonka

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/real0xSI/tiny-chess-gonka/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/real0xSI/tiny-chess-gonka/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

Gonka-search: a 4 KB Python chess engine that plays at ~1654 Elo in local grading (4 wins, 2 draws, 0 losses vs the house trial set). Search-heavy design: negamax with alpha-beta pruning, transposition table, aggressive quiescence search, SEE-lite, MVV-LVA move ordering, killer/history heuristics, LMR, null-move pruning, aspiration windows and check extensions. Evaluation is material + piece-square tables with bishop-pair and endgame king terms, on a 0x88 board with incremental Zobrist hashing. Pure Python 3.13 standard library, deterministic fixed node budget — no clock, no randomness. Packed to 4,044 bytes with the make.fun kit's compress command.

## Run it

```sh
python3 -P -s main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=wee8sydw&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
