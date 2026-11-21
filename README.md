[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Wahyupurnomoaji21/tiny-chess-01-v11/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Wahyupurnomoaji21/tiny-chess-01-v11/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

[Tiny Chess 01 bounty on make.fun](https://make.fun/bounty/tiny-chess-01)

# Tiny Chess Engine v11

From-scratch 0x88 engine (4,079 bytes, Python stdlib only): PVS +
transposition table + null-move pruning + LMR + quiescence + check
extension; material + piece-square eval with pawn-shield king safety and
tapered king value; eval-conditional root repetition filter. Fixed
90,000-node budget per move (deterministic, no clock).

## v11 recipe

Eval v4 (full pawn-advancement table) + search v10 (check extension,
eval-gated repetition filter) + 90k node budget. Killers dropped to fit
the 4,096-byte cap; history + MVV-LVA + TT-move ordering remain.

## Practice trials (kit, 3 trials x 6 games, 90k nodes)

See `~/workspace/makefun/tiny-chess-01-dev/trials-v11/`.
