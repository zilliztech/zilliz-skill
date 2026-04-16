# alias — Create and manage collection aliases.

_Section: Data Operations_

## Prerequisites

- `zilliz` CLI installed and authenticated.
- Active cluster context for operations that target a cluster.

## Commands Reference

### Create — Create an alias pointing to a collection.

```bash
zilliz alias create --collection <collection> --alias <alias>
#   [--database <database>]
#   [--api-key <api-key>]
```

**Flags:**
- `--collection` (**required**, `string`) — target collection name
- `--alias` (**required**, `string`) — alias name
- `--database` (`string`) — database name
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### List — List all aliases.

```bash
zilliz alias list --database <database>
#   [--collection <collection>]
#   [--api-key <api-key>]
```

**Flags:**
- `--database` (**required**, `string`) — database name
- `--collection` (`string`) — filter by collection name
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Describe — Get details of an alias.

```bash
zilliz alias describe --alias <alias>
#   [--database <database>]
#   [--api-key <api-key>]
```

**Flags:**
- `--alias` (**required**, `string`) — alias name
- `--database` (`string`) — database name
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Alter — Reassign an alias to another collection.

```bash
zilliz alias alter --collection <collection> --alias <alias>
#   [--database <database>]
#   [--api-key <api-key>]
```

**Flags:**
- `--collection` (**required**, `string`) — new target collection
- `--alias` (**required**, `string`) — alias name to reassign
- `--database` (`string`) — database name
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Drop — Drop an alias.

```bash
zilliz alias drop --alias <alias>
#   [--database <database>]
#   [--api-key <api-key>]
```

**Flags:**
- `--alias` (**required**, `string`) — alias name to drop
- `--database` (`string`) — database name
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)
