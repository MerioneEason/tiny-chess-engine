# Tiny chess engine

A chess engine in a single Python file (`main.py`, 3,435 bytes, standard
library only). It plays through the make.fun environment: iterative-deepening
alpha-beta search with a transposition table (three-state bound flags),
principal-variation search, late-move reductions, null-move pruning,
quiescence over captures, promotions and check evasions, killer and history
move ordering, and a piece-square-table evaluation under a fixed
55,000-node-per-move budget, so every move is deterministic.
