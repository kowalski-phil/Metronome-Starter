# SUCCESS — what a finished plan looks like

A plan file (`wargames/plan.md`) is DONE only when all 8 criteria hold:

1. Every move states its expected observation on success AND on failure.
2. Every move carries its most likely failure mode, the warning signals,
   and a concrete counter-move.
3. Every fork has an explicit trigger: "if you observe X, take route A, else route B".
4. Each phase has an optimistic assumption AND a pessimistic assumption.
5. Each phase has verifiable exit criteria and a token budget.
6. The master failure table covers every declared area (production & time
   budget, packaging quality, audience response & how to read it,
   platform/algorithm, AI pipeline/tooling, executor discipline, streak
   protection/motivation), with detection and recovery for each row.
7. Every assumption that research could not resolve is flagged as a
   (VARIABLE) placeholder. Nothing is silently guessed.
8. The file ends with abort conditions: the states where the plan stops
   instead of pushing on.

Status rules:
- DONE = all 8 criteria met AND an honest attempt was made to break the plan.
- BLOCKED = two refinement rounds in a row improved nothing.
  List the inputs needed to unblock in LEDGER.md.
