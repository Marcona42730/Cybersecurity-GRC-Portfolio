---
[⬅️ Back to Main Portfolio Root](https://github.com/Marcona42730/Cybersecurity-GRC-Portfolio/blob/main/README.md) | [📂 Governance Module Overview](https://github.com/Marcona42730/Cybersecurity-GRC-Portfolio/tree/main/Governance)
---


# Enterprise Identity & Access Management (IAM) Standard


| Document Version | 1.0.0 |
| :--- | :--- |
| **Owner** | Cybersecurity GRC / IT Governance |
| **Target Audience** | All Employees, Contractors, System Administrators |
| **Regulatory Alignment** | ISO/IEC 27001:2022 (A.5.15, A.5.18), NIST CSF v2.0 (PR.AA-01), RA 10173 DPA, BSP Circular 1086 |
---

### 1. Control Framework Mapping Table

| Control ID | Framework Reference | Policy Requirement Summary |
| :--- | :--- | :--- |
| **IAM-01** | **ISO 27001: A.5.15** | Role-Based Access Control (RBAC) must enforce the Principle of Least Privilege. |
| **IAM-02** | **NIST PR.AA-01** | Multi-Factor Authentication (MFA) is mandatory for all remote and privileged sign-ins. |
| **IAM-03** | **RA 10173 / NPC** | User access logs for systems processing Personal Identifiable Information (PII) must be retained for audit trails. |
| **IAM-04** | **BSP Circular 1086** | Privileged access credentials must undergo quarterly Access Review Certifications. |

---


# 🏛️ Enterprise Identity & Access Management (IAM) Standards
**Scope:** Multi-Platform Financial Operations & Compliance Oversight
**Experience Alignment:** BPI Direct BanKo, Security Bank, GCCS Associates, Billease, Street Lending
**Regulatory Framework:** BSP Circular 454 & 808/1019 | Data Privacy Act of 2012

## 1. Role-Based Access Control (RBAC) Framework
Access is strictly governed by job function and organizational hierarchy to maintain the "Principle of Least Privilege."

* **Frontline/Telecollector Level (Street Lending / Billease):**
    * **Standard:** Least Privilege Access. 
    * **Control:** Access is restricted to assigned customer queues within the **CRM**. Technical controls prevent the export of sensitive contact lists to protect company intellectual property.
* **Specialist/Analyst Level (BPI Direct BanKo / Security Bank):**
    * **Standard:** Segregation of Duties (SoD).
    * **Control:** **Credit Risk Analysts** and **Collection Specialists** have access mapped to their specific portfolios. "Write" access is restricted to prevent unauthorized financial adjustments.
* **Supervisory/Leadership Level (GCCS Associates):**
    * **Standard:** Administrative Oversight & Project-Specific Access.
    * **Control:** As a **Supervisor/Back-Up Leader**, granted oversight authority for the **RCBC Insurance** project. This includes administrative rights within the **Volare** and **ERP** systems for case reassignment and performance auditing.

## 2. System Federation & Data Integrity
To secure high-volume financial data, access to all legacy and modern systems is centralized.

* **Primary Systems:** **Volare (Collections Tool)**, **ERP (Enterprise Resource Planning)**, and **CRM**.
* **Identity Protocol:** Centralized via **Microsoft 365 Single Sign-On (SSO)**. 
* **GRC Logic:** Integrating **Volare** and **ERP** with M365 ensures that a single identity controls access to the entire lifecycle of a debt—from the initial credit risk assessment to final collections.

## 3. Authentication & Device Security
* **MFA Standard:** Mandatory **Microsoft Authenticator** for all systems containing customer financial data (Volare, CRM, ERP).
* **Information Protection:** Access is restricted to managed, encrypted devices to prevent the exfiltration of customer records to unapproved cloud storage or personal hardware.

## 4. Ethical Compliance: Fair Debt Collection Practices
In alignment with **BSP Circular 454**, strict technical and behavioral controls are implemented to prevent Unfair Debt Collection practices.

* **Communication Governance:** Systems are configured to restrict collection calls to authorized hours, and all interactions via **Volare** or the **CRM** are timestamped and recorded.
* **Leadership Oversight (GCCS Associates):** As a **Supervisor**, I performed regular audit reviews of recorded sessions and ERP notes to ensure team adherence to the **Fair Debt Collection Reform Act**.
* **GRC Outcome:** Reduced reputational risk for clients by maintaining a 100% compliance rate during internal quality audits.

---


*Status: Professional Governance & Ethics Standard Implemented*


---
[⬆️ Return to Top](#) | [⬅️ Back to Portfolio Root](https://github.com/Marcona42730/Cybersecurity-GRC-Portfolio/blob/main/README.md)
---
