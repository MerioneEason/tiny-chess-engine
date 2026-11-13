# Tiny chess engine

A chess engine in a single Python file (`main.py`, 3,459 bytes, standard
library only). It plays through the make.fun environment: iterative-deepening
alpha-beta search with a size-capped transposition table (three-state bound
flags, cleared whole once it passes 100,000 entries),
principal-variation search, late-move reductions, null-move pruning,
quiescence over captures, promotions and check evasions, killer and history
move ordering, and a piece-square-table evaluation under a fixed
38,000-node-per-move budget, so every move is deterministic and the
search's memory and time stay well inside the trial limits.
