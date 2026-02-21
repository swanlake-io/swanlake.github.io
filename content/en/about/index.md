---
title: About SwanLake
linkTitle: About
description: Project overview and goals.
menu: { main: { weight: 10 } }
---

{{% blocks/cover
  title="About SwanLake"
  height="auto td-below-navbar"
  image_anchor="bottom"
%}}

SwanLake is an Arrow Flight SQL server backed by DuckDB with DuckLake support.
{.display-6}

{{% /blocks/cover %}}

{{% blocks/lead color="white" %}}

SwanLake focuses on a practical server runtime for analytics and ingestion workloads:
- Arrow Flight SQL for high-throughput SQL over gRPC
- DuckDB for embedded analytical execution
- DuckLake integrations for data lake storage patterns

{{% /blocks/lead %}}

{{% blocks/section %}}

## What You Can Build

- Lakehouse-style query services on top of Postgres and object storage
- Fast ingestion pipelines for logs, events, and operational metrics
- Internal analytics endpoints with simple deployment and operational controls

## Status and Observability

SwanLake includes a status page to inspect active sessions and latency metrics.

![SwanLake Status Page](/images/status_page.png)

{{% /blocks/section %}}
