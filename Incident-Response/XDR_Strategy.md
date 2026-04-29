# 🛡️ Microsoft Defender XDR Defense Strategy
**Target Sector:** Financial Services / Philippine Banking
**Operational Context:** BPI Direct BanKo & Security Bank Experience
**Framework Alignment:** NIST CSF v2.0 (Detect & Respond)

## 1. Objective
To implement a unified security operations (SecOps) strategy using the Microsoft Defender XDR suite. This project demonstrates how to transition from siloed security tools to a coordinated defense-in-depth model, specifically designed to protect banking operational data and ensure system availability according to BSP standards.

## 2. Technical Control Mapping (Risk-Based)
| Security Control | Technical Implementation | Banking Risk Mitigation |
| :--- | :--- | :--- |
| **Defender for Office 365** | Safe Links / Attachment Sandboxing | Neutralizes phishing and Business Email Compromise (BEC) targeting internal bank staff. |
| **Defender for Endpoint** | EDR / Device Control Policies | Blocks unauthorized USB devices and detects malware on data-processing workstations. |
| **Defender for Identity** | UEBA / Identity Protection | Monitors for "Pass-the-Hash" and lateral movement targeting internal bank admin accounts. |
| **Defender for Cloud Apps** | SaaS Visibility / DLP | Prevents unauthorized data exfiltration to unapproved cloud storage or personal portals. |

## 3. Operational Workflow & Governance
* **Automated Containment:** High-risk endpoints are automatically isolated from the bank's production network to prevent the spread of ransomware or unauthorized data access.
* **Audit Transparency:** All security telemetry is consolidated in the Microsoft Defender Portal, serving as primary evidence for BSP (Bangko Sentral ng Pilipinas) regulatory examinations and internal GRC audits.

---
*Target Milestone: 60% Completion (MS-SC-900 Unit 3)*
