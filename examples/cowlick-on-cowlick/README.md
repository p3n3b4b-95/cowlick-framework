# Applying Cowlick to Cowlick

This verified example shows how Cowlick's
[core workflow](../../docs/core-workflow.md) was used to turn its own principles
into repository-level contributor instructions. The completed change is commit
`48f76a2` (`docs: dogfood the Cowlick workflow`).

## Goal

Make Cowlick directly usable by AI tools and contributors working in this
repository while keeping the framework vendor-neutral and documentation-only.

## Inputs

- The six-step [core workflow](../../docs/core-workflow.md).
- The repository structure and principles in the [README](../../README.md).
- The contribution record in the [changelog](../../CHANGELOG.md).
- An existing `.cowlick/config.yml` identifying this as a Cowlick project.

## Decisions

### 1. Frame

The outcome was a working agreement for changes to this repository. The scope
was limited to contributor instructions and the documents that expose and
record them. Runtime code, dependencies, CLI commands, and automation were
explicitly excluded.

The main risk was creating rules that contradicted the vendor-neutral core or
claimed enforcement the repository did not have.

### 2. Inspect

The core workflow, README, changelog, and existing project configuration were
read before editing. There were no callers, tests, fixtures, exports, or runtime
configuration to update because the repository contained documentation only.

### 3. Choose

A root [AGENTS.md](../../AGENTS.md) was the smallest complete change. It reused
the six existing workflow steps and repository structure instead of adding a
new specification, hook, installer, or validation tool.

### 4. Execute

The change added `AGENTS.md`, documented dogfooding in the root README, and
created an `Unreleased` changelog entry. No framework principle or runtime
behavior changed.

### 5. Verify

The change was checked with `git diff --check`, every relative Markdown link
was resolved locally, and the complete diff was reviewed before commit. Commit
`48f76a2` contains only the three intended files.

### 6. Record

The working agreement lives at the repository root where supported AI tools and
contributors can find it. The README explains why it exists, and the changelog
records the addition for the next release.

## Result

Cowlick now uses Cowlick for its own development. A human still owns scope,
safety, and release decisions; the instructions guide work but do not enforce
it automatically.

## Known limits

- `AGENTS.md` is directly consumed only by tools that support it.
- The instructions do not technically prevent a contributor from bypassing the
  workflow.
- Link verification was run manually; the repository still has no automated
  documentation checks.

