# user — Create and manage database users. (Dedicated only)

_Section: Data Operations_

## Prerequisites

- `zilliz` CLI installed and authenticated.
- Active cluster context for operations that target a cluster.

## Commands Reference

### Create — Create a new database user.

```bash
zilliz user create --user <user> --password <password>
#   [--api-key <api-key>]
```

**Flags:**
- `--user` (**required**, `string`) — username
- `--password` (**required**, `string`) — password
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### List — List all database users.

```bash
zilliz user list
#   [--api-key <api-key>]
```

**Flags:**
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Describe — Get details of a user.

```bash
zilliz user describe --user <user>
#   [--api-key <api-key>]
```

**Flags:**
- `--user` (**required**, `string`) — username
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Drop — Drop a database user.

```bash
zilliz user drop --user <user>
#   [--api-key <api-key>]
```

**Flags:**
- `--user` (**required**, `string`) — username to drop
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Update Password — Update user password.

```bash
zilliz user update-password --user <user> --password <password> --new-password <new-password>
#   [--api-key <api-key>]
```

**Flags:**
- `--user` (**required**, `string`) — username
- `--password` (**required**, `string`) — current password
- `--new-password` (**required**, `string`) — new password
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Grant Role — Grant a role to a user.

```bash
zilliz user grant-role --user <user> --role <role>
#   [--api-key <api-key>]
```

**Flags:**
- `--user` (**required**, `string`) — username
- `--role` (**required**, `string`) — role name to grant
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)

### Revoke Role — Revoke a role from a user.

```bash
zilliz user revoke-role --user <user> --role <role>
#   [--api-key <api-key>]
```

**Flags:**
- `--user` (**required**, `string`) — username
- `--role` (**required**, `string`) — role name to revoke
- `--api-key` (`string`, env `ZILLIZ_API_KEY`) — API key (overrides env/config)
