# Docs room: spec text and upstream proposals

One job: draft `DESIGN.md` spec changes before they go upstream. Paths are relative to the
repo root.

## Inputs

- A precedence, canonical-role, or token-format question surfaced while using this fork or
  while building `~/Projects/atelier/spec/DESIGN.md.spec.md`.
- Current spec: `docs/spec.md`. Current proposal: `docs/proposals/precedence-and-canonical-
roles.md` (matches the active branch name).
- Missing input: a proposal with no example behind it (see `examples/CONTEXT.md`) is
  unverified — write the example first or say so in the proposal.

## Process

1. Edit `docs/spec.md` or add a new file under `docs/proposals/` for a distinct proposal.
2. Verify the proposal against at least one fixture in `../examples/`.
3. When the proposal is ready for Atelier, hand it to `atelier/docs/upstream-pr-draft.md` (a
   separate repo, separate room) — this room does not duplicate that file.

## Outputs

- Edited `docs/spec.md`, new/edited `docs/proposals/*.md`.

## Human check

Alex confirms a proposal's claim against the example it cites before it moves to Atelier's
upstream PR draft. Pass: the example demonstrates the claim. Fail: revise the proposal.
