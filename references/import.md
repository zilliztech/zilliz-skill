# import — Import data from cloud storage.

_Section: Cloud Management_

## Prerequisites

- `zilliz` CLI installed and authenticated.
- Active cluster context for operations that target a cluster.

## Commands Reference

### Start — Start a data import job.

```bash
zilliz import start --cluster-id <cluster-id> --collection <collection>
#   [--api-key <api-key>]
```

**Flags:**
- `--cluster-id` (**required**, `string`) — target cluster ID
- `--collection` (**required**, `string`) — target collection name
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### List — List import jobs for a cluster.

```bash
zilliz import list --cluster-id <cluster-id>
#   [--page-size <page-size>]
#   [--page <page>]
#   [--database <database>]
#   [--api-key <api-key>]
```

**Flags:**
- `--cluster-id` (**required**, `string`) — cluster ID
- `--page-size` (`integer`) — items per page
- `--page` (`integer`) — page number
- `--database` (`string`) — database name
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Status — Get status of an import job.

```bash
zilliz import status --job-id <job-id> --cluster-id <cluster-id>
#   [--api-key <api-key>]
```

**Flags:**
- `--job-id` (**required**, `string`) — import job ID
- `--cluster-id` (**required**, `string`) — cluster ID
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)
