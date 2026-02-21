---
title: Configuration
weight: 3
description: Environment variables and runtime tuning.
---

SwanLake loads settings from environment variables with the `SWANLAKE_` prefix.

## Core Server

| Variable | Default | Purpose |
| --- | --- | --- |
| `SWANLAKE_HOST` | `0.0.0.0` | gRPC bind address |
| `SWANLAKE_PORT` | `4214` | gRPC listen port |
| `SWANLAKE_MAX_SESSIONS` | `100` | Max concurrent sessions |
| `SWANLAKE_SESSION_TIMEOUT_SECONDS` | `900` | Idle session cleanup timeout |
| `SWANLAKE_SESSION_ID_MODE` | `peer_addr` | Session identifier mode |

## Status and Metrics

| Variable | Default | Purpose |
| --- | --- | --- |
| `SWANLAKE_STATUS_ENABLED` | `true` | Enable status HTTP server |
| `SWANLAKE_STATUS_HOST` | `0.0.0.0` | Status bind address |
| `SWANLAKE_STATUS_PORT` | `4215` | Status port |
| `SWANLAKE_METRICS_SLOW_QUERY_THRESHOLD_MS` | `5000` | Slow query threshold |
| `SWANLAKE_METRICS_HISTORY_SIZE` | `200` | Metrics history retention |

## DuckLake and DuckDB

| Variable | Default | Purpose |
| --- | --- | --- |
| `SWANLAKE_DUCKLAKE_INIT_SQL` | _(unset)_ | SQL to run after DuckDB startup |
| `SWANLAKE_DUCKDB_THREADS` | DuckDB default | Override execution thread count |

## Maintenance Checkpointing

| Variable | Default | Purpose |
| --- | --- | --- |
| `SWANLAKE_CHECKPOINT_DATABASES` | _(unset)_ | Comma-separated DB list |
| `SWANLAKE_CHECKPOINT_INTERVAL_HOURS` | `24` | Checkpoint interval |
| `SWANLAKE_CHECKPOINT_POLL_SECONDS` | `300` | Poll interval |

For the full and most up-to-date list, see [`CONFIGURATION.md`](https://github.com/swanlake-io/swanlake/blob/main/CONFIGURATION.md).
