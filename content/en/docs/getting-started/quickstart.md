---
title: Quick Start
weight: 1
description: Run SwanLake and connect with a client.
---

## Prerequisites

- Rust toolchain (for local source builds), or Docker
- Open ports `4214` (Flight SQL) and `4215` (status page)

## Run SwanLake Server

From the SwanLake repository root:

```bash
RUST_LOG=info cargo run --bin swanlake
```

Or run the container image:

```bash
docker run --rm -p 4214:4214 -p 4215:4215 ghcr.io/swanlake-io/swanlake:latest
```

## Connect with CLI

```bash
cargo run --bin swanlake-cli --features="cli"
```

By default this connects to `grpc://127.0.0.1:4214`.

## Verify Status Page

Open `http://127.0.0.1:4215` to inspect:
- active sessions
- latency percentiles
- slow queries and recent errors

## Language Examples

- Go ADBC example: [`examples/go-adbc`](https://github.com/swanlake-io/swanlake/tree/main/examples/go-adbc)
- Rust ADBC example: [`examples/rust-adbc`](https://github.com/swanlake-io/swanlake/tree/main/examples/rust-adbc)
- Python examples: [`examples/python-adbc`](https://github.com/swanlake-io/swanlake/tree/main/examples/python-adbc)
