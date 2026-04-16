---
name: zilliz
description: >-
  Manage Zilliz Cloud vector databases via zilliz-cli. Use when the user wants
  to

  set up zilliz-cli, manage clusters and collections, run vector search, import
  or

  back up data, or administer users/roles. Triggers on: zilliz, vector database,

  semantic search, RAG, Milvus, clusters, collections, vector search,
  embeddings.
---
# zilliz — zilliz-cli Skill

Manage Zilliz Cloud clusters and Milvus vector databases via the `zilliz` CLI.

**CLI version:** 1.1.0 (local)

## Prerequisites

- `zilliz` CLI installed. Run `/zilliz:setup` or follow `references/setup.md`.
- Authenticated via `zilliz login`.
- An active cluster context (`zilliz context set` / `zilliz context current`).

## Command pattern

```
zilliz <resource> <operation> [--flag value ...]
```

All commands accept global flags: `-o/--output` (json|table|text|yaml|csv), `--query` (JMESPath), `--no-header`. Resource operations also accept `--api-key` (or `ZILLIZ_API_KEY`), `-a/--all`, `--wait`.

## Reference Files

| Resource | When to read |
|---|---|
| [`cluster`](references/cluster.md) | Create, scale, and manage cloud clusters. |
| [`project`](references/project.md) | Create and manage projects. |
| [`backup`](references/backup.md) | Create, restore, and manage backups. |
| [`import`](references/import.md) | Import data from cloud storage. |
| [`volume`](references/volume.md) | Manage data volumes. |
| [`job`](references/job.md) | Query status of async Cloud Jobs. |
| [`billing`](references/billing.md) | View usage, invoices, and billing information. |
| [`collection`](references/collection.md) | Create and manage vector collections. |
| [`vector`](references/vector.md) | Search, insert, and query vector data. |
| [`database`](references/database.md) | Create and manage databases. |
| [`index`](references/index.md) | Create and manage vector indexes. |
| [`partition`](references/partition.md) | Create and manage collection partitions. |
| [`user`](references/user.md) | Create and manage database users. (Dedicated only) |
| [`role`](references/role.md) | Create and manage access control roles. (Dedicated only) |
| [`alias`](references/alias.md) | Create and manage collection aliases. |

## Top-level commands

- `zilliz configure set` — Set a configuration value
- `zilliz configure get` — Get a configuration value
- `zilliz configure list` — List all configuration values
- `zilliz configure clear` — Clear all stored credentials
- `zilliz context set` — Set the current cluster context
- `zilliz context current` — Show the current context
- `zilliz context clear` — Clear the current context
- `zilliz auth status` — Show current authentication status
- `zilliz auth switch` — Switch to a different organization
- `zilliz login` — Log in to Zilliz Cloud.
- `zilliz logout` — Log out and clear stored credentials.
- `zilliz completion install` — Install shell completion to RC file
- `zilliz completion uninstall` — Remove shell completion from RC file
- `zilliz completion status` — Check if shell completion is installed
- `zilliz completion show` — Print completion script to stdout
- `zilliz version` — Show CLI version.
