# project — Create and manage projects.

_Section: Cloud Management_

## Prerequisites

- `zilliz` CLI installed and authenticated.
- Active cluster context for operations that target a cluster.

## Commands Reference

### Create — Create a new project.

```bash
zilliz project create --name <name> --plan <plan>
#   [--api-key <api-key>]
```

**Flags:**
- `--name` (**required**, `string`) — project name
- `--plan` (**required**, `string`) — [Standard, Enterprise, BusinessCritical]subscription plan
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### List — List all projects.

```bash
zilliz project list
#   [--api-key <api-key>]
```

**Flags:**
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Describe — Get details of a project.

```bash
zilliz project describe --project-id <project-id>
#   [--api-key <api-key>]
```

**Flags:**
- `--project-id` (**required**, `string`) — project ID
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Upgrade — Upgrade project plan.

```bash
zilliz project upgrade --project-id <project-id> --plan <plan>
#   [--api-key <api-key>]
```

**Flags:**
- `--project-id` (**required**, `string`) — project ID
- `--plan` (**required**, `string`) — [Standard, Enterprise, BusinessCritical]target plan
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)
