# design-md-fork

> Status: active | Type: fork (design-token spec experiments)

Local fork of Google Labs' `DESIGN.md` spec, used to draft precedence and canonical-role
proposals that feed `~/Projects/atelier/spec/DESIGN.md.spec.md` and its upstream PR to
`google-labs-code/design.md`. Not a standalone product.

## Where to go

This repo follows ICM (Jake Van Clief's folder method): this file routes, each room's
`CONTEXT.md` holds its contract.

| Task                                                 | Go to       | Read                                       | Skills |
| ---------------------------------------------------- | ----------- | ------------------------------------------ | ------ |
| Change the CLI (`bun run packages/cli/src/index.ts`) | `packages/` | [packages/CONTEXT.md](packages/CONTEXT.md) | none   |
| Draft or update a spec proposal                      | `docs/`     | [docs/CONTEXT.md](docs/CONTEXT.md)         | none   |
| Check a proposal against a real design system        | `examples/` | [examples/CONTEXT.md](examples/CONTEXT.md) | none   |

Root files stay where their tools expect them: `package.json`, `turbo.json`,
`tsconfig.base.json`, `bun.lock` (bun/turbo workspace root), `skills-lock.json`, `.agents/`
(agent skill pins), `README.md`, `CONTRIBUTING.md`, `LICENSE`.

## Naming

TypeScript modules per `packages/cli/src/` convention (camelCase files), docs kebab-case `.md`.
