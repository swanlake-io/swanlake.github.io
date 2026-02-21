---
title: Architecture
weight: 4
description: High-level server and client design.
---

## Core Components

- `swanlake-server`: binary crate that boots and serves Flight SQL.
- `swanlake-core`: shared runtime, config, SQL handlers, session management, metrics.
- `swanlake-client`: Rust client library and CLI.

## Request Flow

1. A Flight SQL client connects over gRPC.
2. SwanLake resolves/creates a session.
3. Statements execute through DuckDB with configured extensions.
4. Results stream back as Arrow data.

## Session Model

SwanLake sessions are connection-affine and own server-side state. For parallelism, clients use multiple gRPC connections via pool abstractions.

## Operational Surface

- Metrics and status page for runtime visibility
- Config via environment variables and `.env`
- Optional background maintenance checkpointing for DuckLake databases
