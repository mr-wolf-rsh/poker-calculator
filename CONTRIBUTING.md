# Contributing

Notes for whoever maintains this hub (currently me). The README is for visitors; this file is
the workflow.

## Adding a new language

1. Create `poker-calculator-<language>`.
2. Implement the algorithm described in [`spec.md`](spec.md) against
   [`fixtures/pokerdata.txt`](fixtures/pokerdata.txt).
3. Add tests covering the hand rankings listed in the spec.
4. Replace that language's row in the hub README table with a link to the new repository, and
   flip its status to ✅ only once the tests pass against the shared fixtures.

## Rules for the shared files

- `fixtures/pokerdata.txt` is the canonical input. Do not edit it in place; add a separate
  fixture file if new cases are needed.
- The spec is the single definition of the exercise. If an implementation disagrees with it,
  the implementation is wrong — unless the spec is what changed, in which case all
  implementations get updated together.

## Known follow-up

The output shape has not been verified as identical across all four implementations yet.
`spec.md` states the intended contract; confirming convergence is outstanding.
