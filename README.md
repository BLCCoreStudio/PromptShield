# PromptShield

**Focused prompt-risk scanning research for AI coding workflows.**

> **Companion research status:** PromptShield's current deterministic prompt-risk rules have been integrated into [AgentGuard](https://github.com/BLCCoreStudio/AgentGuard). This repository remains public as a focused research/reference implementation; new integrated policy, prompt-risk, and sandbox work targets AgentGuard.

PromptShield scans text files for explainable indicators that content may be trying to override an AI agent's instructions, solicit secrets, or trigger unsafe tool use.

## Current development preview

```text
promptshield scan <FILE>
```

The current rules look for a deliberately small set of high-signal phrases and invisible bidirectional-control characters. Findings are warnings for human review, not proof that content is malicious.

## Why this repository still exists

PromptShield is intentionally retained rather than deleted or republished. It preserves the narrow experiment and its development history, keeps existing links valid, and makes the prompt-risk rule set easy to inspect independently from AgentGuard's execution-policy and isolation layers.

For active integration work, use **AgentGuard**.

## Goals

- local-only scanning
- rule IDs with explanations
- low-noise defaults
- no execution of scanned content
- no upload of repository data
- clear distinction between suspicious text and confirmed exploitation

## Build

Requires Rust 1.74 or newer.

```bash
cargo build
cargo test
```

## Security

See [SECURITY.md](SECURITY.md).

## License

MIT © BLC Core Studio
