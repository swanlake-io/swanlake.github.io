---
title: Deployment
weight: 5
description: Run SwanLake in containers and CI environments.
---

## Container Deployment

Use the published image from GitHub Container Registry:

```bash
docker run --rm -p 4214:4214 -p 4215:4215 ghcr.io/swanlake-io/swanlake:latest
```

Set environment variables to control server behavior, status endpoint, and integrations.

## Docker Compose Example

The repository includes `docker-compose.yml` for local orchestration.

## Recommended Runtime Checks

- Probe gRPC endpoint on port `4214`
- Probe status endpoint on port `4215`
- Track p95/p99 latencies and slow query counts from the status page

## CI/CD

- Build and test from the main repository workflows
- Publish container images from tagged releases
- Keep the docs site deployed from `swanlake.github.io` repository
