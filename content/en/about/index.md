---
title: About SwanLake
linkTitle: About
description: Project overview and goals.
menu: { main: { weight: 10 } }
---

{{% blocks/cover
  title="About SwanLake"
  color="swanlake"
  height="auto td-below-navbar"
%}}

SwanLake is an Arrow Flight SQL server backed by DuckDB with DuckLake support.
{.display-6}

<div class="td-cta-buttons my-5">
  <a class="btn btn-lg btn-primary" href="/docs/getting-started/quickstart/">
    Quick Start
  </a>
  <a class="btn btn-lg btn-secondary" href="https://github.com/swanlake-io/swanlake" target="_blank" rel="noopener noreferrer">
    GitHub
    <i class="fa-brands fa-github px-1"></i>
  </a>
</div>

{{% blocks/link-down %}}

{{% /blocks/cover %}}

{{% blocks/lead color="white" %}}

<h2 class="display-4 font-weight-bold mb-4">Practical Analytics Runtime</h2>

<p class="lead text-muted">SwanLake focuses on providing a high-performance, simple, and extensible server for modern data workloads.</p>

{{% /blocks/lead %}}

{{% blocks/section color="primary" %}}

<div class="container mt-4">
<div class="row g-5">
<div class="col-lg-4 text-left">
<div class="feature-card">
<div class="feature-icon"><i class="fa-solid fa-bolt"></i></div>
<h3>Arrow Flight SQL</h3>
<p>High-throughput SQL over gRPC, optimized for low-latency data transfer and ingestion.</p>
</div>
</div>
<div class="col-lg-4 text-left">
<div class="feature-card">
<div class="feature-icon"><i class="fa-solid fa-microchip"></i></div>
<h3>DuckDB Execution</h3>
<p>Embedded analytical execution engine for lightning-fast query processing on local and remote data.</p>
</div>
</div>
<div class="col-lg-4 text-left">
<div class="feature-card">
<div class="feature-icon"><i class="fa-solid fa-water"></i></div>
<h3>DuckLake Integration</h3>
<p>Native support for data lake storage patterns, bridging the gap between local compute and cloud storage.</p>
</div>
</div>
</div>
</div>

{{% /blocks/section %}}

{{% blocks/section color="white" %}}

<div class="container">
<div class="row align-items-center">
<div class="col-lg-6 text-left">
<h2 class="display-4 mb-4">What You Can Build</h2>
<p class="lead opacity-75 mb-4">SwanLake is designed to be a versatile component in your data infrastructure.</p>
<ul class="list-unstyled">
<li class="mb-3 d-flex align-items-start text-left">
<i class="fa-solid fa-circle-check text-success mt-1 mr-3"></i>
<span><strong>Lakehouse Services:</strong> Query services on top of Postgres and object storage.</span>
</li>
<li class="mb-3 d-flex align-items-start text-left">
<i class="fa-solid fa-circle-check text-success mt-1 mr-3"></i>
<span><strong>Ingestion Pipelines:</strong> Fast pipelines for logs, events, and operational metrics.</span>
</li>
<li class="mb-3 d-flex align-items-start text-left">
<i class="fa-solid fa-circle-check text-success mt-1 mr-3"></i>
<span><strong>Analytics Endpoints:</strong> Internal endpoints with simple deployment and controls.</span>
</li>
</ul>
</div>
<div class="col-lg-6">
<div class="swanlake-home-visual p-0 m-0">
  <img src="/images/swanlake.jpeg" alt="SwanLake visual" loading="lazy" />
</div>
</div>
</div>
</div>

{{% /blocks/section %}}

{{% blocks/section color="secondary" %}}

<div class="container">
<div class="row align-items-center">
<div class="col-lg-6 order-lg-2 text-left">
<h2 class="display-4 text-white mb-4">Status & Observability</h2>
<p class="lead text-light opacity-75 mb-4">Built-in visibility into your server's health and performance.</p>
<p class="text-light opacity-75 mb-0">SwanLake includes a dedicated status page to inspect active sessions, track query latency (P95/P99), monitor slow queries, and analyze system errors in real-time.</p>
</div>
<div class="col-lg-6 order-lg-1">
<div class="swanlake-home-visual m-lg-0 mt-5 mt-lg-0">
  <img src="/images/status_page.png" alt="SwanLake Status Page" loading="lazy" />
</div>
</div>
</div>
</div>

{{% /blocks/section %}}
