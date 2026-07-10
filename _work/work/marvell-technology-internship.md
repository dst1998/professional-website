---
layout: page
title: Marvell Technology
description: Solutions Architecture Intern
start_date: 2026-05
end_date: Present
importance: 1
category: work
---

- Built a full-stack memory tiering simulation system and co-design for large-scale AI workloads in hyperscalers.
- Implemented a multi-tier heterogeneous memory hierarchy spanning from local GPU-attached memory through CXL-pooled DRAM and local storage to remote network-attached storage, with per-operator placement policies and Chakra trace-driven tier routing for LLM inference workloads.
- Designed a backward-compatible extension to the MLCommons Chakra memory node standard, making memory semantics explicit and tier-aware by enriching memory nodes with operation type, workload role, tier direction, access patterns, and near-memory compute hooks to drive a simulation pipeline.
- Extended CXL memory pool and near-memory compute accelerator simulators into ASTRA-sim's memory simulation infrastructure as live in-process latency models, covering cross-NPU coherency miss modeling, congestion analysis, and near-memory compute offload evaluation; calibrated against Marvell CXL hardware.
- Presented at the AstraSim Tutorial at ISCA 2026 on enabling memory tiering in ASTRA-sim with extended Chakra traces, covering LLM serving workloads including KV cache offload, LoRA adapter swap, and weight prefetch; proposed as an upstream contribution to MLCommons Chakra.

