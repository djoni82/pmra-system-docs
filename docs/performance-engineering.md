# Performance engineering

Measured engineering capability supported by technical evidence. Every published measurement states its scope and limitations.

- **PMRA-BENCH-001 — 168-Hour Reliability Test** (VERIFIED). 168 hours, 1–8 October 2026; 20,093 samples; 0 recorded errors; 0 restarts. Controlled read-only market data workload. Measures reliability and continuity; it does not represent trading, fill or latency performance.
- **PMRA-BENCH-002 — Archived High-Throughput Engineering Test** (ARCHIVED / PARTIALLY VERIFIED). 16 March 2026: 13.5M market data events processed; 16+ hours continuous operation with 0 recorded errors; shared-memory IPC throughput up to 946K msg/s; SBE encode 1.1 µs. Historical engineering environment; it does not represent the current runtime or order round-trip latency. The SBE figure measures encode time, distinct from acknowledgment time.
- **PMRA-BENCH-003 — Authentication Signing Microbenchmark** (PARTIALLY VERIFIED). HMAC-SHA256 request signing, p99.9 0.180 µs. Component-level measurement only; it does not represent end-to-end tick-to-trade or order-acknowledgment latency.
- **Packet-path engineering** (UNDER VALIDATION). AF_PACKET and AF_XDP receive paths have been evaluated in controlled laboratory tests. Kernel-bypass deployment remains under validation and is not deployed in the current runtime.

No public end-to-end tick-to-trade number is published. Detailed environment and methodology are available for qualified review.
