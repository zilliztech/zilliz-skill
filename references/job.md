# job — Query status of async Cloud Jobs.

_Section: Cloud Management_

## Prerequisites

- `zilliz` CLI installed and authenticated.
- Active cluster context for operations that target a cluster.

## Commands Reference

### Describe — Get status of an async job (backup, restore, migration, import, etc.).

```bash
zilliz job describe --job-id <job-id>
#   [--api-key <api-key>]
```

**Flags:**
- `--job-id` (**required**, `string`) — job ID (e.g. job-xxxxxxxxxxxxxxxxxxxx)
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)
