---
title: SwanLake
description: Arrow Flight SQL server backed by DuckDB and DuckLake.
params:
  body_class: td-navbar-links-all-active
---

{{% blocks/lead color="white" %}}

<div class="swanlake-home-video">
  <div class="ratio ratio-16x9">
    <iframe
      src="https://www.youtube.com/embed/XVm3sptCfCA"
      title="SwanLake introduction video"
      loading="lazy"
      referrerpolicy="strict-origin-when-cross-origin"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen
    ></iframe>
  </div>
</div>

{{% /blocks/lead %}}

{{% blocks/section color="primary" %}}

<div class="container mt-4">
<div class="row g-5">
<div class="col-lg-4">
<div class="feature-card">
<div class="feature-icon">
<i class="fa-solid fa-rocket"></i>
</div>
<h3>Arrow Flight SQL</h3>
<p>Low-latency SQL access over gRPC for analytics and ingestion workloads. Optimized for high-throughput data transfer.</p>
</div>
</div>
<div class="col-lg-4">
<div class="feature-card">
<div class="feature-icon">
<i class="fa-solid fa-database"></i>
</div>
<h3>DuckDB + DuckLake</h3>
<p>Harness the power of DuckDB execution with DuckLake-backed storage. Native patterns for Postgres and object storage.</p>
</div>
</div>
<div class="col-lg-4">
<div class="feature-card">
<div class="feature-icon">
<i class="fa-solid fa-chart-line"></i>
</div>
<h3>Built-In Status Page</h3>
<p>Real-time visibility into active sessions, latency metrics, slow query logs, and system error analysis.</p>
</div>
</div>
</div>
</div>

{{% /blocks/section %}}

{{% blocks/section color="secondary" %}}

<div class="container">
<div class="row align-items-center">
<div class="col-lg-6 mb-5 mb-lg-0 text-left">
<h2 class="display-4 text-white">Start in Minutes</h2>
<p class="lead text-light mb-4 opacity-75">Launch SwanLake locally or with Docker and start querying your data instantly with Arrow Flight SQL.</p>
<ul class="list-unstyled text-left">
<li class="mb-2 text-light"><i class="fa-solid fa-check text-success mr-2"></i> No complex configuration</li>
<li class="mb-2 text-light"><i class="fa-solid fa-check text-success mr-2"></i> Native DuckDB performance</li>
<li class="mb-2 text-light"><i class="fa-solid fa-check text-success mr-2"></i> gRPC-based connectivity</li>
</ul>
</div>
<div class="col-lg-6">

```bash
# Run server from source
RUST_LOG=info cargo run --bin swanlake

# Or run with Docker
docker run --rm -p 4214:4214 -p 4215:4215 \
  ghcr.io/swanlake-io/swanlake:latest
```

<div class="mt-4 small text-light opacity-50">
<p class="mb-1"><strong>Default endpoints:</strong></p>
<ul class="list-inline">
<li class="list-inline-item mr-3">Flight SQL: <code>grpc://127.0.0.1:4214</code></li>
<li class="list-inline-item">Status page: <code>http://127.0.0.1:4215</code></li>
</ul>
</div>

</div>
</div>
</div>

{{% /blocks/section %}}
