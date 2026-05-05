# 📁 Data Governance & Information Protection
**Scope:** Customer PII Management (Banking, Insurance, & Fintech)
**Technical Framework:** Microsoft Purview & Microsoft Priva
**SC-900 Alignment:** Unit 4 - Microsoft Compliance Solutions

## 1. Information Protection (Microsoft Purview)
To ensure compliance with **BSP Circular 808** and the **Data Privacy Act**, we utilize Sensitivity Labels to classify data based on risk.

* **Label: [Highly Confidential] - Banking Records**
    * **Application:** CRM exports, loan applications, and RCBC Insurance records.
    * **Control:** Encryption is mandatory; "Print" and "Forward" functions are disabled via Purview.
* **Label: [Confidential] - Operational Data**
    * **Application:** Supervisor notes and team performance metrics in the ERP/Volare.
    * **Control:** Access is restricted to GCCS Leadership and authorized Analysts only.

## 2. Data Loss Prevention (DLP)
DLP policies are implemented to prevent the unauthorized exfiltration of sensitive financial data.

* **DLP Trigger:** Identification of 16-digit credit card numbers or bank account formats.
* **Policy Action:** Blocks the email or upload to **Dropbox** and alerts the Supervisor.
* **GRC Purpose:** Mitigates "Insider Risk" and ensures zero-leakage of customer debt records.

## 3. Privacy Risk Management (Microsoft Priva)
Utilizing **Microsoft Priva** to automate privacy risk mitigation for the Collections team.
* **Data Minimization:** Automated detection of over-retained PII within SharePoint or local workstations.
* **Leadership Oversight:** As a **Supervisor**, I leverage Priva alerts to ensure that frontline collectors are only accessing the specific customer data required for their current queue.

---
*Status: Compliance Module Implemented (SC-900 Unit 4)*
