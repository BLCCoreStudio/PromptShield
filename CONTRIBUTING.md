# Contributing

Focused detection rules, false-positive reductions, Unicode edge cases, tests, and documentation improvements are welcome.

Before opening a pull request:

```bash
cargo fmt --all -- --check
cargo clippy --all-targets -- -D warnings
cargo test --all-targets
```

Every new detection rule should be explainable and include both positive and negative tests where practical. Security reports belong in the private channel described by `SECURITY.md`.
