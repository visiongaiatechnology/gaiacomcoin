# VGT-OMEGA PROTOCOL: GaiaComCoin (GCC)
> **Post-Quantum Sovereign Value Transfer Protocol**

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen)](https://github.com/VisionGaiaTechnology/gaiacomcoin)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)
[![Status](https://img.shields.io/badge/status-BETA%20(TESTNET)-orange)](STATUS)

## ⚠️ CLASSIFIED DEVELOPMENT PREVIEW
**WARNUNG:** Dies ist eine **Phase 3 Beta (Testnet)** Implementierung.  
Die kryptographischen Primitive (Kyber1024/Dilithium5) sind sicherheitstechnisch scharf geschaltet, aber das Netzwerk-Peering erfordert manuelle Konfiguration. Nutzen Sie dies NICHT für Echtwert-Transaktionen.

## 🏛 Architecture: The Hybrid Shield
GCC implementiert eine kompromisslose "Defense in Depth" Strategie gegen Quantencomputer-Bedrohungen:
* **KEM:** X25519 + Kyber1024 (Hybrid Handshake)
* **DSA:** Ed25519 + Dilithium5 (Hybrid Signatures)
* **Consensus:** VGT-Matrix (Memory-Hard / Latency-Hard Proof-of-Work)
* **Engine:** Rust (Edition 2024), Zero-Panic Policy, Sled DB Persistence.

## 🚀 Getting Started (Testnet Node)

### Prerequisites
* Rust (latest stable)
* C-Compiler (gcc/clang) für PQ-Crypto Bindings
* OpenSSL dev libs

### Installation
```bash
git clone [https://github.com/VisionGaiaTechnology/gcc-core.git](https://github.com/VisionGaiaTechnology/gcc-core.git)
cd gcc-core/backend
cargo build --release
Running a Node
Starten Sie einen Seed-Node (generiert Genesis-Block):

Bash

./target/release/gcc_node --seed --p2p-port 8333 --api-port 8080
Starten Sie einen Peer und verbinden Sie ihn manuell:

Bash

./target/release/gcc_node --p2p-port 8334 --api-port 8081 --connect 127.0.0.1:8333

🗺 Roadmap Status
[x] Phase 1: Zero Point (Core Architecture, Hybrid Crypto)

[x] Phase 2: The Network (P2P Protocol, Binary Wire Format)

[x] Phase 3: The Consensus (VGT-Matrix Mining, Chainstate Persistence)

[ ] Phase 4: Mainnet Launch (Active Peer Discovery, Governance Activation, Audit)
