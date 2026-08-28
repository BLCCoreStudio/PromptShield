# PromptShield

**Local scanner for prompt-injection patterns targeting AI coding agents.**

> **Status:** early development. No stable release has been published.

PromptShield scans text files for explainable indicators that content may be trying to override an AI agent's instructions, solicit secrets, or trigger unsafe tool use.

## Current development preview

```text
promptshield scan <FILE>
```

The first rules look for a deliberately small set of high-signal phrases and invisible bidirectional-control characters. Findings are warnings for human review, not proof that content is malicious.

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
