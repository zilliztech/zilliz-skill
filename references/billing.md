# billing — View usage, invoices, and billing information.

_Section: Cloud Management_

## Prerequisites

- `zilliz` CLI installed and authenticated.
- Active cluster context for operations that target a cluster.

## Commands Reference

### Usage — Show billing usage summary.

```bash
zilliz billing usage
#   [--month <month>  # default: today]
#   [--last <last>]
#   [--start <start>]
#   [--end <end>]
```

**Flags:**
- `--month` (`string`, default `today`) — Month: YYYY-MM, 'this', or 'last'
- `--last` (`string`) — Relative period: 7d, 1m, 1y
- `--start` (`string`) — Start time (ISO 8601 or YYYY-MM-DD)
- `--end` (`string`) — End time (ISO 8601 or YYYY-MM-DD)

### Invoices — List invoices.

```bash
zilliz billing invoices
#   [--page-size <page-size>  # default: 20]
#   [--page <page>  # default: 1]
```

**Flags:**
- `--page-size` (`integer`, default `20`) — Number of invoices per page
- `--page` (`integer`, default `1`) — Page number
