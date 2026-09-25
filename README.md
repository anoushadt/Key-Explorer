# Key Explorer

**Key Explorer** is the comprehensive cryptographic toolkit for professional developers, security engineers, and PKI administrators in IntelliJ IDEA. Inspect, edit, analyze, convert, and manage certificates, keystores, and keys directly within your IDE workflow.

---

## Important Update: Transition to Freemium Model

To accelerate development, support emerging cryptographic standards (including Post-Quantum Cryptography), and deliver enterprise-grade features, Key Explorer is transitioning to a **Freemium** model.

> [!IMPORTANT]
> **All existing core features remain 100% Free forever!**
> Opening, viewing, inspecting, and analyzing certificates, keystores, private and public keys, CSRs, CRLs, validating chains, and classical format conversions will always remain free.

Advanced enterprise and modern cryptographic capabilities — including Post-Quantum Cryptography (PQC & Hybrid), in-place Keystore editing, Hardware Security Module (PKCS#11 HSM) integration, internal CA issuance, ACME / Let's Encrypt automation, and dedicated Pro workspace tools — are now available under **Key Explorer Pro**, with a **30-day fully functional free trial**.

---

## Free vs. Pro Feature Comparison

| Feature Area | Feature | Key Explorer (Free) | Key Explorer Pro |
|---|---|:---:|:---:|
| **Certificates** | X.509 Certificate Viewer (PEM, DER, PKCS#7, PKIPath) | ✅ Included | ✅ Included |
| **Certificates** | Chain Validation & Trust Store Path Verification | ✅ Included | ✅ Included |
| **Certificates** | Extension Decoding (SAN, Key Usage, Basic Constraints, etc.) | ✅ Included | ✅ Included |
| **Keystores** | Keystore Viewer (PKCS#12, JKS, JCEKS, BKS, UBER) | ✅ Included | ✅ Included |
| **Keystores** | In-Place Keystore Editing (Unlock, Add, Delete, Save) | ❌ | ⭐️ **Pro** |
| **Keystores** | Master Password Storage Integration | ✅ Included | ✅ Included |
| **Keys** | Classical Key Inspection (RSA, EC, Ed25519 PKCS#1/PKCS#8) | ✅ Included | ✅ Included |
| **PQC** | Post-Quantum Cryptography (ML-DSA, ML-KEM, SLH-DSA, Falcon) | ❌ | ⭐️ **Pro** |
| **PQC** | Composite & Hybrid Cryptography (e.g. MLDSA87-Ed448) | ❌ | ⭐️ **Pro** |
| **PQC** | Quantum Readiness Assessment & Algorithm Scoring | ❌ | ⭐️ **Pro** |
| **HSM** | PKCS#11 Hardware Security Modules & SoftHSM Browsing | ❌ | ⭐️ **Pro** |
| **PKI** | Local Certificate Authority (CA) Management & Issuance | ❌ | ⭐️ **Pro** |
| **PKI** | ACME / Let's Encrypt Client (Automated Request & Renewal) | ❌ | ⭐️ **Pro** |
| **Standards** | ASN.1 Hierarchy & Hex Inspector | ✅ Included | ✅ Included |
| **Standards** | CSR (Certificate Signing Request) & CRL Inspection | ✅ Included | ✅ Included |
| **Standards** | CBOR, COSE, and CWT Export | ❌ | ⭐️ **Pro** |
| **Workspace** | Multi-Tab Tool Window Workspace with Drag-and-Drop | ✅ Included | ✅ Included |
| **Workspace** | Classical Format Export (PEM, DER, PKCS#12, Chains) | ✅ Included | ✅ Included |
| **Workspace** | Verify Host TLS Certificates | ❌ | ⭐️ **Pro** |
| **Workspace** | Cryptographic Key–Cert Pair Validator | ❌ | ⭐️ **Pro** |
| **Licensing** | 30-Day Free Trial Available | — | **Yes (1-click)** |

---

## Getting Started

### Installation
1. Open IntelliJ IDEA (or any compatible JetBrains IDE: Ultimate, Community, PyCharm, WebStorm, GoLand, etc.).
2. Navigate to **Settings / Preferences &rarr; Plugins &rarr; Marketplace**.
3. Search for **Key Explorer** and click **Install**.
4. Restart your IDE if prompted.

### Starting your 30-Day Free Trial
You can try all Pro features without restrictions for 30 days:
1. Open **Settings / Preferences &rarr; Plugins &rarr; Installed &rarr; Key Explorer**.
2. Click **Manage Licenses...** and choose **Start 30-Day Free Trial**.
3. Alternatively, click **"Start 30-Day Free Trial"** on any Pro action card or notification in the IDE.

---

## Feature Overview

### 1. Core Free Features

#### Certificate Viewer
Decode and inspect X.509 certificates in all common representations:
- Supported encodings: PEM, DER, PKCS#7 (`.p7b`, `.p7c`, `.spc`), and PKIPath (`.pkipath`).
- Inspect standard properties (Subject, Issuer, Serial Number, Validity, Signature Algorithm).
- Generate fingerprints (SHA-1, SHA-256) with one click.
- Interactive certificate chain navigation.

#### Keystore Navigator
Explore Java and standard keystores without complex `keytool` terminal commands:
- Supported formats: PKCS#12 (`.p12`, `.pfx`), JKS (`.jks`), JCEKS (`.jceks`), BKS, and UBER.
- Browse all aliases, view certificate chains, and inspect private key parameters.

#### Key & CSR Inspector
- Inspect RSA, ECDSA, and Ed25519 keys (PKCS#1 and PKCS#8).
- Parse Certificate Signing Requests (CSRs) and Certificate Revocation Lists (CRLs).

#### ASN.1 Tree & Hex Analyzer
- Deep dive into the underlying ASN.1 structure with a collapsible tree.
- Inspect raw bytes, tags, lengths, and hexadecimal payloads.

#### Tool Window Workspace
- Docked side-panel workspace with multi-tab support.
- Open files via toolbar button or by dragging and dropping directly into the panel.
- Export classical certificates, chains, public keys, and private keys into PEM or DER formats.

---

### 2. Key Explorer Pro Features

#### Post-Quantum & Hybrid Cryptography (PQC)
- Full support for NIST FIPS 203/204/205 standards:
  - **ML-KEM** (Kyber): 512, 768, 1024
  - **ML-DSA** (Dilithium): 44, 65, 87
  - **SLH-DSA** (SPHINCS+): SHA2 and SHAKE variants
  - **Falcon**: 512, 1024
  - **Stateful hash-based signatures**: LMS, HSS, XMSS, XMSS^MT
- **Composite & Hybrid Signatures:** Support for hybrid keys and certificates (e.g. `MLDSA87-Ed448-SHAKE256`), combining classical algorithms with quantum-safe primitives.
- **Quantum Readiness Scoring:** Automated audit of cryptographic assets with actionable migration recommendations.

#### In-Place Keystore Editing
- Unlock keystores within your editor.
- Add new keys, import certificates, change passwords, and delete aliases.
- Save modified keystores directly back to disk or re-encrypt into other formats.

#### Hardware Security Module (HSM) Integration
- Direct integration with PKCS#11 hardware devices and SoftHSM.
- Browse tokens, explore slots, and view hardware-backed certificates without external utilities.

#### Local Certificate Authority (CA) & ACME
- Establish local root and intermediate CAs for local development and testing.
- Sign CSRs and issue certificates with custom extensions and validity periods.
- Native ACME / Let's Encrypt client for automated certificate acquisition and renewal.

#### Advanced Workspace Utilities
- **Verify TLS:** Fetch and validate live certificate chains from any remote host and port.
- **Key–Cert Pair Validator:** Cryptographically verify that a private key matches a given certificate before deployment.
- **CBOR, COSE, and CWT:** Parse, validate, and export modern IoT and web-token payloads.

---

## Building from Source

To build and test the plugin locally:

```bash
# Clone the repository
git clone https://github.com/xkrypt-com/Key-Explorer.git
cd Key-Explorer

# Run tests
./gradlew test

# Package and prepare IDE sandbox
./gradlew shadowJar obfuscate prepareSandbox

# Launch a test IDE instance with Key Explorer loaded
./gradlew runIde
```

---

## License & Support

- **Vendor:** xkrypt
- **Website:** [https://xkrypt.com](https://xkrypt.com)
- **Support:** [hello@xkrypt.com](mailto:hello@xkrypt.com)
- **Documentation:** See `docs/marketplace/` for full guides and Custom Pages.

---

## Trademarks & Third-Party Notices

- **Thales**, **Luna**, **SafeNet**, and **Chrystoki** are trademarks or registered trademarks of Thales Group or its affiliates.
- **SoftHSM** is maintained by OpenDNSSEC / NLnet Labs.
- **Let's Encrypt** is a trademark of the Internet Security Research Group (ISRG).
- **JetBrains**, **IntelliJ**, and **IntelliJ IDEA** are trademarks or registered trademarks of JetBrains s.r.o.

*Key Explorer is an independent product developed by xkrypt and is not affiliated with, endorsed by, or sponsored by Thales Group, JetBrains, or any other trademark holder mentioned herein.*
