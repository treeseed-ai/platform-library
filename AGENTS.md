# Project library guidance

This repository is the authoritative Git history for one TreeSeed project library. TreeDX remains the canonical query and authoring service; do not edit TreeDX storage or `.treeseed/data` directly.

Use `trsd library show <project>` and `trsd library status <project>` to discover the binding and verify its exact upstream and index state. Use `trsd library paths`, `read`, `search`, `query`, and `context` with the project slug and, when reproducibility matters, `--ref <exact-commit>`.

Library collections live at repository root, for example `agents/`, `books/`, `knowledge/`, `notes/`, and `questions/`. Do not recreate `src/content`; Astro consumers map an immutable TreeDX or object-storage projection into their own content integration.

Save knowledge through `trsd library workspace create`, `read`, `write`, `diff`, and `submit`. Review and publish through `trsd library reviews`. Never push an unreviewed TreeDX authoring ref, expose provider credentials, silently accept a moved ref, or treat an empty result from an unhealthy binding as authoritative.
