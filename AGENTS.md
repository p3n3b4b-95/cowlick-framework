# Cowlick contributor instructions

This repository uses Cowlick to develop Cowlick. Follow the
[core workflow](docs/core-workflow.md) for every change:

1. Frame the outcome, constraints, risks, and exclusions.
2. Inspect every affected document and reuse the repository's language and
   structure.
3. Choose the smallest complete, maintainable change.
4. Keep execution focused; do not add speculative features or tooling.
5. Verify changed claims, commands, and relative links.
6. Record notable work under `Unreleased` in `CHANGELOG.md`.

## Repository rules

- Keep the core framework vendor-neutral; put tool-specific guidance in
  `adapters/`.
- Put repeatable procedures in `playbooks/` and reusable decisions in
  `patterns/`.
- Examples must state their goal, inputs, decisions, verification, and limits.
- Do not add a runtime, dependency, automation, or CLI until repeated use proves
  it is needed.
- A human owns scope, safety, and release decisions.

Before finishing, stage the intended files, run `git diff --check` and
`git diff --cached --check`, confirm relative Markdown links resolve, and
review the complete staged diff.
