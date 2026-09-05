# PromptShield

> **Project status: sunset / discontinued.**

PromptShield was a focused prompt-risk scanning experiment for AI coding workflows. Its deterministic rules were later integrated into AgentGuard, which has itself now been discontinued as BLCCoreStudio reduces overlapping experimental projects.

The repository remains public for historical reference and to preserve existing links and commit history, but **no further feature development or routine maintenance is planned**.

## Historical scope

PromptShield scanned text files for explainable indicators that content might be attempting to override an AI agent's instructions, solicit secrets, or trigger unsafe tool use. Findings were designed as human-review warnings rather than proof that content was malicious.

The project focused on:

- local-only scanning;
- deterministic rule IDs and explanations;
- a small set of high-signal patterns;
- detection of invisible bidirectional-control characters;
- no execution of scanned content;
- no upload of repository data;
- explicit separation between suspicious text and confirmed exploitation.

## Historical source

Previous implementation details, tests, documentation, and development history remain available through the Git history.

## License

MIT © BLC Core Studio
