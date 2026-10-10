# Cowlick Framework

**Engineering Framework for AI-assisted Development**

> Think Once. Build Anywhere.

Cowlick is a vendor-neutral engineering framework for consistent collaboration
between people and AI across software development, automation, operations, and
system design.

## Principles

- **Engineer first** — AI assists; people remain accountable for decisions.
- **Think first** — understand the problem before generating a solution.
- **Verify first** — test claims and outputs instead of assuming they are right.
- **Native first** — prefer existing platform capabilities before integrations.
- **Reuse first** — adapt proven work before creating more.
- **Simplicity wins** — choose the smallest maintainable solution.

Cowlick is independent of AI vendors and tools. ChatGPT, Claude, Codex, Gemini,
Cursor, and other systems can act as execution engines; Cowlick defines the
engineering workflow around them.

## Repository map

| Path | Purpose |
| --- | --- |
| `.cowlick/` | Project-level Cowlick metadata and configuration |
| `docs/` | Framework documentation |
| `examples/` | Small, complete examples |
| `playbooks/` | Repeatable, outcome-focused procedures |
| `patterns/` | Reusable engineering patterns |
| `adapters/` | Guidance for specific AI tools |

## Start here

1. Read the [core workflow](docs/core-workflow.md).
2. Copy `.cowlick/config.yml` into a project and adjust its name.
3. Add only the playbooks, patterns, and adapters that project needs.
4. Keep a human responsible for review, verification, and release decisions.

## Contributing

Contributions are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) and the
[Code of Conduct](CODE_OF_CONDUCT.md) before opening an issue or pull request.

## License

Licensed under the [Apache License 2.0](LICENSE). It is permissive and includes
an explicit patent grant, making it a strong default for a community engineering
framework.

