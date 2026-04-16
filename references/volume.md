# volume — Manage data volumes.

_Section: Cloud Management_

## Prerequisites

- `zilliz` CLI installed and authenticated.
- Active cluster context for operations that target a cluster.

## Commands Reference

### Create — Create a new volume.

```bash
zilliz volume create --project-id <project-id> --region <region> --name <name>
#   [--api-key <api-key>]
```

**Flags:**
- `--project-id` (**required**, `string`) — project ID
- `--region` (**required**, `string`) — cloud region (e.g. aws-us-west-2)
- `--name` (**required**, `string`) — volume name
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### List — List all volumes in a project.

```bash
zilliz volume list --project-id <project-id>
#   [--page-size <page-size>]
#   [--page <page>]
#   [--api-key <api-key>]
```

**Flags:**
- `--project-id` (**required**, `string`) — project ID
- `--page-size` (`integer`) — items per page
- `--page` (`integer`) — page number
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Delete — Delete a volume.

```bash
zilliz volume delete --name <name>
#   [--api-key <api-key>]
```

**Flags:**
- `--name` (**required**, `string`) — volume name to delete
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)
