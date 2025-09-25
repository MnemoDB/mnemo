# Mnemo

<p align="center">
  <img src="MnemoLogo.png" alt="Mnemo Logo" width="200"/>
</p>

**Mnemo** is a rich in-memory database written in Rust, fully compatible with
the Redis protocol (RESP3) and designed to extend beyond Redis OSS with the
entire Redis Stack feature set — including JSON, Search, TimeSeries, Bloom
filters, and Vector similarity.

## Features
- ⚡ RESP3 wire-compatibility — works with existing Redis clients.
- 📦 Core data types — Strings, Lists, Hashes, Sets, Sorted Sets, Streams.
- ⏱️ Expiry & eviction policies (LRU, LFU, Random).
- 💾 Persistence — RDB snapshots & AOF with background rewrite.
- 🔄 Replication & Cluster mode (hash slots, failover).
- 📊 Redis Stack — JSON documents, full-text search, time series, bloom/CF/TopK, vector indexing.
- 🔐 ACL, TLS, scripting (Lua/JS).

## Roadmap
- [ ] Phase 0: Core RESP3 server (`PING`, `SET`, `GET`, TTL, INFO).
- [ ] Phase 1: Core data types, AOF/RDB.
- [ ] Phase 2: Replication & Cluster.
- [ ] Phase 3: JSON + Search + Vector.
- [ ] Phase 4: TimeSeries + Bloom suite.
- [ ] Phase 5: HA polish (Sentinel-like, ACL, TLS, scripting).

## Philosophy
Mnemo is built with three principles:
1. **Compatibility** — drop-in replacement for Redis/Redis Stack.
2. **Performance** — memory-efficient, low-latency, multi-core scaling.
3. **Extensibility** — modular crates (JSON, Search, TS) for evolving workloads.

## License
Apache 2.0