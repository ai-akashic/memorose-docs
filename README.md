# Memorose Docs

Documentation site for Memorose, built with Mintlify.

This repository documents the current `memorose-server` HTTP API, runtime model, deployment patterns, and contributor workflows.

## Local development

Install the Mintlify CLI:

```bash
npm i -g mint
```

Run the local preview from the repo root:

```bash
mint dev
```

The preview runs at `http://localhost:3000`.

## Link checks

Run broken-link validation before publishing documentation changes:

```bash
mint broken-links
```

## Source of truth

This docs repo should follow the current code in the main Memorose repository.

When docs and examples conflict, prefer:

- `Memorose/crates/memorose-server/src/main.rs`
- `Memorose/crates/memorose-server/src/types.rs`
- `Memorose/crates/memorose-common/src/config.rs`
- `Memorose/README.md`

## What this docs set covers

- `getting-started/`: installation, quickstart, and runtime configuration
- `api/`: current `v1` HTTP routes
- `architecture/`: memory hierarchy, storage model, and deployment model
- `guides/`: operational and integration workflows
- `contributing/`: local development, testing, codebase structure, and dashboard internals
- `sdks/`: HTTP-first client-wrapper guidance for language-specific users

## Writing guidance

- Document the current runtime, not older CRUD-style memory APIs.
- Prefer explicit route names and request fields over vague conceptual summaries.
- Keep English and Chinese pages aligned when changing product behavior or API semantics.
