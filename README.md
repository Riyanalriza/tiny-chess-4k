# tiny-chess-4k

A chess engine in at most 4 KB of Python, built for the make.fun
[tiny-chess-01](https://make.fun) bounty: build the strongest chess engine
in 4 KB of Python.

`main.py` (3,844 bytes) is the whole engine: a 0x88 board, complete move
generation, alpha-beta with a transposition table, quiescence, MVV-LVA and
killer move ordering, and a piece-square-table evaluation, searching to a
fixed 100,000 nodes per move. Deterministic: no clock, no randomness, no
model calls. Python 3.13 standard library only.

Practice Elo measured on the kit's own gauntlet: 1451 (trial-0), 1364
(trial-1). The readable source is `engine.py` (kept in the working folder;
`main.py` is its compressed form).

MIT licensed.
