# Packages room: the design-monorepo CLI

One job: change the CLI that exercises the `DESIGN.md` spec experiments. Paths are relative to
the repo root.

## Inputs

- A change tied to a spec proposal in `docs/proposals/` or a fixture in `examples/`.
- Code: `packages/cli/src/`, `packages/cli/scripts/`.
- Missing input: NOT FOUND — no test directory was found under `packages/cli/`; confirm with
  Alex whether tests exist before assuming `turbo test` covers this package.

## Process

1. Make the change in `packages/cli/src/`.
2. `bun run packages/cli/src/index.ts` (the `cli` script in root `package.json`) against a
   fixture in `../examples/` to see real output.
3. `turbo build` / `turbo lint` from the repo root before committing.

## Outputs

- Changed `packages/cli/src/*`.

## Human check

Alex runs the CLI against an example and confirms the output matches the proposal it's meant
to implement. Pass: output matches. Fail: fix and re-run.
