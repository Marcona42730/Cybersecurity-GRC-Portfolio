# 🏛️ Identity and Access Management (IAM) Standards
**Scope:** Corporate & BYOD Device Governance
**Control Framework:** Zero Trust Architecture (Verify Explicitly)
**Regulatory Alignment:** BSP Information Security Framework (Circular 808/1019)

## 1. Device Enrollment & Asset Management
To maintain a high-security posture, device compliance state is used as a primary signal for Conditional Access.

* **Microsoft Entra Joined (Corporate-Owned):**
    * **Policy:** Mandatory for all bank-purchased hardware and workstations.
    * **GRC Logic:** Ensures full MDM (Mobile Device Management) enrollment. This enables remote wipe capabilities, BitLocker encryption, and automated patching required for banking audit compliance.
* **Microsoft Entra Registered (BYOD):**
    * **Policy:** Limited to personal mobile devices for basic productivity (Email/Teams) only.
    * **GRC Logic:** Provides identity visibility without administrative control. Access to core banking systems is **strictly prohibited** from Registered devices.

## 2. Authentication & Access Control
* **MFA Requirement:** All employee identities must utilize **Phishing-Resistant MFA** (Microsoft Authenticator with Number Matching) for all sensitive financial data access.
* **Access Principle:** Implementation of **Least Privilege Access (LPA)** based on verified job roles and device health.

## 3. Compliance Enforcement
* **Zero Trust Validation:** Technical confirmation through SC-900 standards that "Entra Joined" is the required state for organizational assets to ensure they are managed under the corporate identity.
* **Control Objective:** To eliminate "Shadow IT" by ensuring only managed, compliant devices can interact with sensitive banking operational data.

---
*Status: Governance Module Verified (Unit 2)*
