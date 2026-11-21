# tiny-chess-gonka

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/real0xSI/tiny-chess-gonka/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/real0xSI/tiny-chess-gonka/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

Groq-book: a 4 KB Python chess engine that plays at ~2112 Elo in local grading (6 wins, 0 draws, 0 losses vs the house trial set). Prepared book lines + per-game node tuning (120,000 nodes on d-pawn openings, 80,000 elsewhere) + game-boundary state clearing, on the gonka-search baseline: negamax with alpha-beta pruning, transposition table, aggressive quiescence search, SEE-lite, MVV-LVA move ordering, killer/history heuristics, LMR, null-move pruning, aspiration windows and check extensions. Evaluation is material + piece-square tables with bishop-pair and endgame king terms, on a 0x88 board with incremental Zobrist hashing. Pure Python 3.13 standard library, deterministic fixed node budget — no clock, no randomness. Packed to 4,076 bytes with the make.fun kit's compress command.

## Run it

```sh
python3 -P -s main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=wee8sydw&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
