# Horizon Protocol

**Horizon Protocol** is an open-source, offline-first decentralized mesh networking protocol written from scratch in Rust. It is engineered to provide resilient, low-overhead peer-to-peer communication without relying on centralized telecom infrastructure.

> **Status:** Active Pre-Release Development (Architecture & Core Engineering Phase)

---

## The Problem

Existing decentralized and peer-to-peer mesh messaging solutions face critical bottlenecks in real-world deployments:
- **Severe battery drain** caused by inefficient scanning and background relaying.
- **Fragile multi-hop routing** that degrades rapidly as node density fluctuates.
- **Bloated third-party dependency chains** that increase attack surfaces and complicate security audits.
- **Poor scalability** beyond isolated local clusters.

## Architectural Pillars

Horizon Protocol takes a clean-slate systems approach with minimal external dependencies:

- **Built from Scratch in Rust:** Guarantees memory safety, zero-cost abstractions, and predictable resource usage on constrained mobile hardware.
- **Hybrid Mesh-to-Gateway Routing:** Bridges local Bluetooth and Wi-Fi device-to-device relay chains with internet gateways, enabling seamless scaling from local clusters to wider regions.
- **Power-Aware Traffic Isolation:** Strictly reserves low-power Bluetooth/mesh relays for lightweight emergency text routing, confining high-bandwidth media and voice to direct internet connections.
- **Resilient Offline Synchronization:** Lightweight local state sync and abuse-resistant relay mechanics designed to operate reliably under intermittent connectivity.

## Target Use Cases

- Disaster-relief and emergency response teams operating in infrastructure-damaged zones.
- Humanitarian organizations requiring auditable, self-contained communication layers.
- Developers seeking an embeddable, open-source mesh networking core.
- Communities facing network outages or restricted telecom access.

## Roadmap

- [x] Core protocol architecture & hybrid routing specification
- [x] Power-aware traffic isolation model
- [ ] Core packet framing and cryptographic handshake layer (Rust)
- [ ] Multi-hop routing engine & local relay state machine
- [ ] Multi-node mesh topology simulator & automated fuzzing suite
- [ ] Public v0.1 alpha release & benchmark reports
- [ ] Security audit & v1.0 stable release

## License

This project is open-source and licensed under the **Apache License 2.0**. See the [LICENSE](LICENSE) file for details.
