---
name: cowlick
description: Apply Cowlick's vendor-neutral engineering workflow when Cowlick is explicitly requested or the current project contains .cowlick/config.yml. Do not use for unrelated projects merely because they involve coding.
---

# Cowlick

Use Cowlick to keep AI-assisted engineering human-owned, focused, and
verifiable.

## Workflow

1. **Frame** the outcome, constraints, risks, and exclusions.
2. **Inspect** every affected caller, document, test, fixture, configuration,
   and export before changing anything.
3. **Choose** the smallest complete, maintainable solution, preferring existing
   project patterns and native capabilities.
4. **Execute** only the scoped change; avoid speculative features and tooling.
5. **Verify** behavior, claims, commands, links, and the complete diff in
   proportion to the risk.
6. **Record** notable decisions and usage guidance where future contributors
   will find them.

## Boundaries

- A human owns scope, safety, and release decisions.
- Keep core guidance vendor-neutral and isolate tool-specific adaptations.
- Do not add a runtime, dependency, integration, or abstraction without a
  demonstrated need.
- Never trade away validation, security, accessibility, or data safety for a
  smaller change.

When adopting Cowlick in a new project, start with only `.cowlick/config.yml`
and project-level contributor instructions. Add playbooks, patterns, examples,
or adapters only when the project actually needs them.

