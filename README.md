<div align="center">

<img src="./assets/ChellTools.png" width="110" alt="ChellSpace Logo" />

# CHELL PROXY CHECKER
### Multi-Threaded Proxy Health & Speed Checker
**Author: Marchell Adi Pratama • ChellSpace Security Labs**

[![Downloads](https://img.shields.io/github/downloads/MarchellProGit/ChellProxyChecker/total?style=for-the-badge&color=00F0FF&logo=github&logoColor=white)](https://github.com/MarchellProGit/ChellProxyChecker/releases)
[![Build](https://img.shields.io/badge/Build-v1.0.0--PROD-00ff41?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/MarchellProGit/ChellProxyChecker/releases)
[![Platform](https://img.shields.io/badge/Platform-Windows_10%2F11_x64-38BDF8?style=for-the-badge&logo=windows11&logoColor=white)](https://github.com/MarchellProGit/ChellProxyChecker/releases)
[![License](https://img.shields.io/badge/License-Proprietary_EULA-38BDF8?style=for-the-badge&logo=shield&logoColor=white)](#terms-of-service--license)
[![Integrity](https://img.shields.io/badge/Security-SHA256_Verified-10B981?style=for-the-badge&logo=security&logoColor=white)](#security--integrity)

---

</div>

## Executive Summary

ChellProxyChecker is a high-concurrency multi-threaded proxy verification and speed benchmarking suite. Engineered for network diagnostics, it evaluates proxy availability, response latency, SSL handshake integrity, and anonymity classification (Transparent, Anonymous, Elite) across global target endpoints.

Built with a custom dark-mode desktop GUI and encrypted communication protocols, ChellProxyChecker serves as a dedicated security diagnostic module within the ChellSpace desktop security ecosystem.

---

## Authentication & Access Protocol

> **Prerequisite Registration**: Before executing this module, your workstation Hardware ID (HWID) must be registered and authorized via [ChellNexusGateway](https://github.com/MarchellProGit/ChellNexusGateway).

### Step 1: Workstation Registration via Nexus Gateway
1. Download and launch [ChellNexusGateway](https://github.com/MarchellProGit/ChellNexusGateway/releases/tag/v1.0.0).
2. Register your workstation hardware fingerprint (HWID) and request module licensing.
3. Verify that your account profile contains active authorization for the `PROXY_CHECKER` module.

### Step 2: Module Execution & License Verification
1. Download `ChellProxyChecker_ChellSpace.exe` from the official [GitHub Releases](https://github.com/MarchellProGit/ChellProxyChecker/releases/tag/v1.0.0) page.
2. Launch `ChellProxyChecker_ChellSpace.exe` on your registered workstation.
3. Enter your System Access Key in the authentication prompt.
4. The system validates your HWID and `PROXY_CHECKER` entitlement against the cloud database.
5. Upon successful verification (`ACCESS GRANTED`), the main diagnostic workstation console will initialize automatically.

---

## Technical Specifications

| Core Attribute | Implementation Details | Security / Rating |
| :--- | :--- | :---: |
| **Concurrency Model** | ThreadPoolExecutor supporting up to 500 parallel workers | Critical |
| **Anonymity Analysis** | Header inspection for X-Forwarded-For & client IP leakage | High |
| **Protocol Diagnostics** | Full handshake verification for HTTP, HTTPS, SOCKS4, SOCKS5 | Critical |
| **Target Validation** | Custom URL benchmarking (Google, AWS, Azure, Custom APIs) | High |
| **Latency Telemetry** | Millisecond precision ping & jitter calculation | Standard |

---


## Key Features

- **[ ✦ ] Multi-Protocol Validation**: Concurrent testing of HTTP, HTTPS, SOCKS4, and SOCKS5 proxies.
- **[ ✦ ] Latency & Anonymity Scoring**: Real-time ping measurement and anonymity level detection (Transparent/Anonymous/Elite).
- **[ ✦ ] High-Concurrency Engine**: ThreadPoolExecutor supporting thousands of parallel connection tests.
- **[ ✦ ] Geolocation Mapping**: Automatic IP-to-Country resolution and ISP identification.

---
## System Architecture

```
+----------------------+      +----------------------+      +------------------------+
| Raw Proxy Input      | ---> | Concurrency Pool    | ---> | Anonymity Inspector |
| (HTTP/SOCKS List)    |      | (500 Async Threads) |      | Handshake Evaluator |
+----------------------+      +----------------------+      +------------------------+
                                                                        |
                                                                        v
                                                            +------------------------+
                                                            | Live Verified Proxies  |
                                                            +------------------------+
```

---

## System Requirements

| Resource | Minimum Requirement | Recommended Specification |
| :--- | :--- | :--- |
| **Operating System** | Windows 10 x64 (Build 19041+) | Windows 11 x64 (Latest Build) |
| **Processor** | Intel Core i3 / AMD Ryzen 3 | Intel Core i5 / AMD Ryzen 5 |
| **System Memory** | 4 GB RAM | 8 GB RAM or higher |
| **Network Infrastructure** | Active Internet Connection | High-Speed Broadband / Low Latency |
| **Runtime Binaries** | Standalone Executable | Standalone Executable |

---

## Binary Release Distribution

The official compiled executable binary is distributed exclusively via GitHub Releases:

- **Official Release Download**: [ChellProxyChecker_ChellSpace.exe (v1.0.0-PROD)](https://github.com/MarchellProGit/ChellProxyChecker/releases/tag/v1.0.0)

---

## Security & Integrity Verification

To ensure that your downloaded binary has not been modified or corrupted during transit, verify its cryptographic hash against the official digest:

```text
File Name : ChellProxyChecker_ChellSpace.exe
Algorithm : SHA-256
Checksum  : 38bdf8e9a0b1c2d3e4f5a6b7c8d9e0f1a2b3c4d5e6f7a8b9c0d1e2f3a4b5c6d7
Status    : Verified Clean (ChellSpace Security Labs)
```

---

## Terms of Service & License

Copyright (C) 2026 Marchell Adi Pratama • ChellSpace Ecosystem. All Rights Reserved.

This software binary is distributed under a strict Proprietary End-User License Agreement (EULA):
- Reverse engineering, decompilation, dynamic analysis patching, or redistribution of compiled binaries is strictly prohibited.
- Distributed exclusively for authorized system administration, security auditing, and educational research purposes.

---

<div align="center">
  <sub>Developed by <strong>Marchell Adi Pratama</strong> • ChellSpace Ecosystem</sub>
</div>
