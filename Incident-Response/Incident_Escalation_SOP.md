# Incident Response & Severity Escalation Standard Operating Procedure (SOP)

| Document Version | 1.0.0 |
| :--- | :--- |
| **Owner** | Cybersecurity Incident Response Team (CIRT) / GRC |
| **Target Audience** | Operations Managers, Team Leads, Helpdesk, Security Operations Center (SOC) |
| **Framework Alignment** | NIST SP 800-61 Rev. 2, ISO/IEC 27001:2022 (Control A.5.24 - A.5.28) |

---

## 1. Purpose & Scope
This Standard Operating Procedure (SOP) defines the operational workflow for detecting, categorizing, escalating, and containing information security incidents. It ensures SLA compliance and clear chain-of-command handoffs during critical operational disruptions.

---

## 2. Severity Level Classification & Escalation SLAs

| Severity Level | Definition / Example Scenario | Response SLA | Required Notification & Escalation Path |
| :--- | :--- | :--- | :--- |
| **SEV-1 (Critical)** | Active ransomware outbreak, confirmed breach of customer PII/financial records, or complete outage of core transaction systems. | **< 15 Mins** | CISO, Data Protection Officer (DPO), Executive Leadership, Legal Team, Regulatory Bodies (e.g., NPC / BSP) within 72 hours. |
| **SEV-2 (High)** | Confirmed compromise of a single privileged account (e.g., Team Lead credentials), malware isolated on a operational workstation. | **< 1 Hour** | Incident Response Team Lead, Operations Manager, IT Security Supervisor. |
| **SEV-3 (Medium)** | Policy non-compliance (e.g., unauthorized USB drive usage), multiple failed login attempts successfully blocked by MFA. | **< 4 Hours** | Tier-2 SOC Analyst, GRC Officer. |
| **SEV-4 (Low)** | Suspicious email report (phishing attempt) with no link clicked, routine system audit flag. | **< 24 Hours** | Service Desk, IT Support. |

---

## 3. Incident Lifecycle Phases (Aligned with NIST SP 800-61)

```text
  [1. Preparation] ──► [2. Detection & Analysis] ──► [3. Containment, Eradication & Recovery] ──► [4. Post-Incident Activity]
