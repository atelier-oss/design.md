# Examples room: reference fixtures

One job: hold real `DESIGN.md` files a proposal or CLI change can be checked against. Paths
are relative to the repo root.

## Inputs

- A proposal in `docs/proposals/` or a CLI change in `packages/cli/` that needs a real fixture
  to prove against.
- Current fixtures: `examples/atmospheric-glass/`, `examples/paws-and-paths/`,
  `examples/totality-festival/`.
- Missing input: a proposal claim with no matching fixture — add one rather than asserting
  the claim untested.

## Process

1. Run `bun run packages/cli/src/index.ts` (or the relevant CLI command) against the fixture
   that exercises the proposal in question.
2. Add a new example folder, matching the existing fixtures' shape, when no current fixture
   covers the case.

## Outputs

- Existing or new `examples/<name>/` folders. Never edit a fixture to make a broken proposal
  pass — fix the proposal or the code instead.

## Human check

Alex confirms the fixture output is what the proposal or CLI change was supposed to produce.
Pass: matches. Fail: the code or the proposal is wrong, not the fixture.
