# ⬡ GaiaComCoin (GCC)

[![Build](https://img.shields.io/badge/Build-Passing-brightgreen?style=for-the-badge)](https://github.com/VisionGaiaTechnology/gaiacomcoin)
[![Status](https://img.shields.io/badge/Status-BETA%20TESTNET-orange?style=for-the-badge)](#)
[![Phase](https://img.shields.io/badge/Phase-3%20Hardened-purple?style=for-the-badge)](#roadmap)
[![Rust](https://img.shields.io/badge/Rust-Edition%202024-CE422B?style=for-the-badge&logo=rust)](https://rust-lang.org)
[![PQC](https://img.shields.io/badge/Crypto-Kyber1024%20%2B%20Dilithium5-blue?style=for-the-badge)](#architecture)
[![VGT](https://img.shields.io/badge/VGT-VisionGaia_Technology-red?style=for-the-badge)](https://visiongaiatechnology.de)
[![Donate](https://img.shields.io/badge/Donate-PayPal-00457C?style=for-the-badge&logo=paypal)](https://www.paypal.com/paypalme/dergoldenelotus)

> *"The first Rust-native protocol with Hybrid Quantum Shield technology — built to fix Bitcoin's architectural weaknesses without sacrificing decentralization."*

---

<img width="1892" height="1900" alt="GaiaComCoin" src="https://github.com/user-attachments/assets/7de5c288-5bc1-457e-b739-9d2e771fe79a" />

---

## ⚠️ Development Preview — Testnet Only

This is a **Phase 3 Beta (Testnet)** implementation. The cryptographic primitives (Kyber1024 / Dilithium5) are fully operational, but network peering requires manual configuration.

**Do NOT use for real-value transactions.**

---

## 🚨 Why GCC Exists

Bitcoin was designed in 2008. Quantum computers were theoretical. Today they are not.

| Bitcoin / Legacy Chains | GaiaComCoin |
|---|---|
| ❌ ECDSA — broken by Shor's algorithm | ✅ Dilithium5 — NIST PQC standard |
| ❌ ECDH — vulnerable to quantum KEM attacks | ✅ Kyber1024 — post-quantum key exchange |
| ❌ C++ — memory unsafe, CVE surface | ✅ Rust 2024 — ownership model, zero-panic policy |
| ❌ SHA256 PoW — ASIC centralization | ✅ VGT-Matrix — memory-hard, latency-bound, ASIC-resistant |
| ❌ No governance layer | ✅ On-chain voting, humanitarian treasury, founder vesting |

---

## 🏛️ Architecture — The Hybrid Shield

GCC implements an uncompromising Defense in Depth strategy against quantum threats. Every layer of the stack is hardened — from key exchange to consensus.

```
┌─────────────────────────────────────────────────────┐
│                    APP CLIENTS                       │
│  Mobile (iOS/Android)  │  Desktop  │  Cold Storage  │
├─────────────────────────────────────────────────────┤
│                  WEB (REACT)                         │
│  Encrypted State  │  Visualization  │  No Raw Keys  │
├─────────────────────────────────────────────────────┤
│               BRIDGE (WASM / Secure Enclave)         │
│  fn generate_secure_identity()                       │
│  Private Key never touches JavaScript                │
├─────────────────────────────────────────────────────┤
│                 BACKEND (RUST 2024)                  │
│  gcc_core (Ledger)  │  gcc_consensus (PoW)           │
│  Sled DB (Storage)  │  Zero-Panic Policy             │
├─────────────────────────────────────────────────────┤
│              ENCRYPTION LAYER                        │
│  Transport: Noise Protocol                           │
│  Storage:   AES-256-GCM                              │
│  KEM:       X25519 + Kyber1024 (Hybrid)              │
│  DSA:       Ed25519 + Dilithium5 (Hybrid)            │
└─────────────────────────────────────────────────────┘
```

---

## 💎 Core Specs

| Parameter | Value |
|---|---|
| **Max Supply** | 71,000,000 GCC (Hard Cap) |
| **Halving** | Every 210,000 blocks |
| **Engine** | Rust Edition 2024 |
| **KEM** | X25519 + Kyber1024 (Hybrid) |
| **DSA** | Ed25519 + Dilithium5 (Hybrid) |
| **Consensus** | VGT-Matrix (Memory-Hard / Latency-Bound PoW) |
| **Storage** | Sled DB (Embedded, Zero-Config) |
| **Transport** | Noise Protocol |
| **ASIC Resistance** | ✅ (Memory-Hard by design) |

---

## 🖥️ Native Client Suite

### 📱 Mobile One — iOS & Android `GPLv3`
Pocket sovereignty. Full SPV Node with governance voting interface and QR-based air-gap signing.
- Biometric authentication
- Governance dashboard
- Air-gap QR signing

### 🖥️ Node Commander — Win / Mac / Linux `GPLv3`
The power tool for network guardians. Integrated full node, mining control and advanced block analysis.
- Integrated miner
- P2P graph visualizer
- Real-time chainstate

### 🔐 VisionBit Zero — Cold Storage OS `GPLv3`
The ultimate fortress. Offline signing software that runs from USB sticks. Private keys never leave the air-gap.
- True offline signing
- Physical entropy generator
- Paper wallet export

---

## 🏛️ Governance & Policy

### The Humans Wallet
**30% of genesis supply (21.3M GCC)** is hard-coded for humanitarian projects. These funds are locked via smart contracts and can only be released through on-chain community voting — maximum 3% per year.

### Founder Vesting
To make rug pulls mathematically impossible, founder coins (7.77%) are subject to strict vesting: **12-month cliff**, followed by **linear release over 5 years** — enforced via `OP_CHECKLOCKTIMEVERIFY`.

### Stealth Development
Specific governance modules remain closed source until mainnet launch to prevent hostile forks and vampire attacks. All governance logic converts to Apache 2.0 automatically on **01.01.2029** (BSL 1.1 Change Date).

---

## 📜 Hybrid License Model

| Component | License | Rationale |
|---|---|---|
| **Core Engine** (Network, Crypto) | Apache 2.0 | Maximum adoption, auditable |
| **Governance Logic** | BSL 1.1 → Apache 2.0 (2029) | Network protection during build phase |
| **Client Suite** (Apps) | GPLv3 | Community contribution enforced |
| **Documentation** | CC BY-SA 4.0 | Free knowledge sharing |

> **BSL 1.1 Clause:** The governance logic automatically converts to Apache 2.0 on 01.01.2029. This protects the network during the critical build phase against commercial copies ("Vampire Attacks").

---

## 🗺️ Roadmap

| Phase | Name | Status |
|---|---|---|
| ✅ Phase 1 | **Zero Point** — Core Architecture, Hybrid Crypto | Complete |
| ✅ Phase 2 | **The Network** — P2P Protocol, Binary Wire Format | Complete |
| ✅ Phase 3 | **The Consensus** — VGT-Matrix Mining, Chainstate Persistence | **Active (88%)** |
| 🔒 Phase 4 | **Mainnet Launch** — Active Peer Discovery, Governance, Audit | Locked |

```
Protocol Development Status
████████████████████░░  88% [Phase 3 Hardened]

Core Engine  : READY
Consensus    : READY
Governance   : PENDING (Locked until Mainnet)
```

---

## 🚀 Getting Started (Testnet Node)

### Requirements
- Rust (latest stable)
- C compiler (gcc / clang) for PQ-Crypto bindings
- OpenSSL dev libs

### Installation

```bash
git clone https://github.com/VisionGaiaTechnology/gcc-core.git
cd gcc-core/backend
cargo build --release
```

### Running a Seed Node (generates Genesis block)

```bash
./target/release/gcc_node --seed --p2p-port 8333 --api-port 8080
```

### Connecting a Peer

```bash
./target/release/gcc_node --p2p-port 8334 --api-port 8081 --connect 127.0.0.1:8333
```

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.

The Core Engine and Client Suite are open source. Governance modules will open on 01.01.2029.

---

## ☕ Support the Project

GCC is developed independently. If you believe in post-quantum sovereign value transfer:

[![Donate via PayPal](https://img.shields.io/badge/Donate-PayPal-00457C?style=for-the-badge&logo=paypal)](https://www.paypal.com/paypalme/dergoldenelotus)

---

## 🏢 Built by VisionGaia Technology

[![VGT](https://img.shields.io/badge/VGT-VisionGaia_Technology-red?style=for-the-badge)](https://visiongaiatechnology.de)

VisionGaia Technology builds enterprise-grade security and AI tooling — engineered to the DIAMANT VGT SUPREME standard.

> *"When quantum computers arrive, most blockchains will not survive the first morning. GCC was built for that morning."*

---

*Version Beta Phase 3 — GaiaComCoin // Post-Quantum Sovereign Protocol*
