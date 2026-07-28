# Information Security Risk Assessment Matrix

## 1. Qualitative Scoring Model
Risk Score is calculated as: **Risk Score = Likelihood (1–5) × Impact (1–5)**

* **Critical Risk (20–25):** Requires immediate executive escalation and remediation within 24 hours.
* **High Risk (12–19):** Remediation required within 7 to 14 days.
* **Medium Risk (6–11):** Remediation scheduled within the quarterly operational sprint.
* **Low Risk (1–5):** Accept risk or address during routine maintenance.

---

## 2. Enterprise Risk Log & Controls Mapping

| Risk ID | Threat Scenario | Asset Impacted | Likelihood (1-5) | Impact (1-5) | Inherent Risk | Mitigation / Security Control | Residual Risk | Regulatory / Framework Mapping |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **RSK-01** | Unauthorized personnel accesses customer financial data due to over-permissioned account. | Core Banking Portal | 4 | 5 | **20 (Critical)** | Implement Role-Based Access Control (RBAC) via Microsoft Entra ID; enforce Least Privilege. | **6 (Medium)** | ISO/IEC 27001 Control A.5.15 / RA 10173 |
| **RSK-02** | Credential harvesting via phishing attack targeting frontline operational staff. | O365 / Corporate Email | 4 | 4 | **16 (High)** | Mandatory FIDO2 / MFA via Microsoft Authenticator; deploy automated anti-phishing in Defender. | **4 (Low)** | NIST CSF PR.AA-05 |
| **RSK-03** | Delayed access revocation for terminated employees (Insider Threat). | Internal Knowledge Base & CRM | 3 | 4 | **12 (High)** | Automate HR Offboarding workflows tied directly to Entra ID account disabling. | **3 (Low)** | ISO/IEC 27001 Control A.5.18 |
