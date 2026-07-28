---
[⬅️ Back to Main Portfolio Root](https://github.com/Marcona42730/Cybersecurity-GRC-Portfolio/blob/main/README.md) | [📂 Technical Security Overview](https://github.com/Marcona42730/Cybersecurity-GRC-Portfolio/tree/main/Technical-Skills)
---

# M365 Security & Identity Control Architecture (SC-900 Alignment)

| Document Version | 1.0.0 |
| :--- | :--- |
| **Owner** | Cybersecurity GRC / Cloud Security Architecture |
| **Target Audience** | Security Engineers, IT Administrators, GRC Auditors |
| **Framework Alignment** | NIST CSF v2.0 (PR.AA, PR.DS), ISO/IEC 27001:2022 (A.5.15, A.8.5), SC-900 |

---

## 1. Overview & Architectural Scope
This document outlines the operational implementation of identity, access, and compliance controls within Microsoft Entra ID and Microsoft 365. It provides technical verification for security controls mapped in `01-Governance` and risk mitigations listed in `02-Risk-Management`.

---

## 2. Core Security Control Matrix

| Security Domain | Applied Feature / Control | Configuration Standard | Operational Purpose |
| :--- | :--- | :--- | :--- |
| **Identity & Access** | **Microsoft Entra Conditional Access** | Require MFA for all users; Block Legacy Authentication protocols. | Prevents credential stuffing and unauthorized remote access. |
| **Zero-Trust Access** | **Role-Based Access Control (RBAC)** | Principle of Least Privilege; Just-In-Time (JIT) access via PIM. | Limits lateral movement and prevents permanent admin privilege creep. |
| **Data Protection** | **Microsoft Purview Information Protection** | Auto-labeling sensitivity rules for PII/Financial data. | Restricts unauthorized download, sharing, or printing of sensitive files. |
| **Threat Protection** | **Microsoft Defender for Endpoint** | Automated Investigation & Response (AIR); EDR enabled. | Quarantines malicious activity automatically at the endpoint level. |

---

## 3. Zero-Trust Access Architecture

```text
[ Incoming Request ] 
        │
        ▼
[ Microsoft Entra ID Conditional Access ]
        │
        ├──► Verification: User Identity + MFA (Microsoft Authenticator)
        ├──► Context: Device Compliance (Intune) + Location/IP Risk
        │
        ├───► [ Block Access ] (If Risk Level = High or Legacy Auth)
        └───► [ Grant Minimal Access ] (Session Monitored)

```

---
[⬆️ Return to Top](#) | [⬅️ Back to Main Portfolio Root](https://github.com/Marcona42730/Cybersecurity-GRC-Portfolio/blob/main/README.md)
---
