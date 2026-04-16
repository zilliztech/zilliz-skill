# role — Create and manage access control roles. (Dedicated only)

_Section: Data Operations_

## Prerequisites

- `zilliz` CLI installed and authenticated.
- Active cluster context for operations that target a cluster.

## Commands Reference

### Create — Create a new role.

```bash
zilliz role create --role <role>
#   [--api-key <api-key>]
```

**Flags:**
- `--role` (**required**, `string`) — role name
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### List — List all roles.

```bash
zilliz role list
#   [--api-key <api-key>]
```

**Flags:**
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Describe — Get details and privileges of a role.

```bash
zilliz role describe --role <role>
#   [--api-key <api-key>]
```

**Flags:**
- `--role` (**required**, `string`) — role name
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Drop — Drop a role.

```bash
zilliz role drop --role <role>
#   [--api-key <api-key>]
```

**Flags:**
- `--role` (**required**, `string`) — role name to drop
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Grant Privilege — Grant a privilege to a role.

```bash
zilliz role grant-privilege --role <role> --object-type <object-type> --object-name <object-name> --privilege <privilege>
#   [--database <database>]
#   [--api-key <api-key>]
```

**Flags:**
- `--role` (**required**, `string`) — role name
- `--object-type` (**required**, `string`) — [Global, Collection, Database]object type
- `--object-name` (**required**, `string`) — object name (or * for all)
- `--privilege` (**required**, `string`) — privilege name (e.g. Search, Insert, CreateCollection)
- `--database` (`string`) — database name
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Revoke Privilege — Revoke a privilege from a role.

```bash
zilliz role revoke-privilege --role <role> --object-type <object-type> --object-name <object-name> --privilege <privilege>
#   [--database <database>]
#   [--api-key <api-key>]
```

**Flags:**
- `--role` (**required**, `string`) — role name
- `--object-type` (**required**, `string`) — [Global, Collection, Database]object type
- `--object-name` (**required**, `string`) — object name (or * for all)
- `--privilege` (**required**, `string`) — privilege name
- `--database` (`string`) — database name
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)
