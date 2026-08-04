# Mock Audit Finding Report

## Audit Overview

**Audit Type:** Internal Security & Access Control Audit  
**Framework Alignment:** NIST SP 800-53 / ISO 27001 / SOC 2 Access Management Principles  
**Audit Period:** Q2 2023  
**Finding Status:** Open - Remediation Required  

> **Auditor Note:**  
> A clean audit is uncommon. Findings are an expected part of a mature security program. The goal of GRC is not simply to identify deficiencies, but to manage risk, determine root cause, implement corrective actions, and validate that controls are operating effectively.

---

# Finding Details

## Finding ID
**DEL-2023-01**

## Control ID
**AC-02 - Account Management**

## Control Area
Identity and Access Management (IAM)

## Control Objective

Ensure user accounts are properly managed throughout the employee lifecycle, including timely provisioning, modification, and termination of access privileges.

---

# Finding Description

During a review of Q2 employee terminations, auditors sampled **15 departed employees** to validate compliance with the organization's access revocation requirements.

Testing identified that:

- **3 out of 15 terminated users** did not have access revoked within the required **24-hour Service Level Agreement (SLA)**.
- Azure Active Directory and GitHub access remained active for an average of **9 days following termination**.
- Offboarding activities were not consistently initiated or tracked through the approved IT workflow.

---

# Affected Systems

| System | Access Type | Impact |
|---|---|---|
| Azure Active Directory | User authentication and cloud resources | Unauthorized account access |
| GitHub Enterprise | Source code repositories | Potential exposure of proprietary code |
| Production environments | Application access pathways | Potential unauthorized changes |

---

# Risk / Business Impact

Failure to promptly disable terminated user accounts creates a risk of unauthorized access to organizational resources.

Potential impacts include:

- Unauthorized access to proprietary source code
- Data exposure or exfiltration
- Unauthorized modifications to production environments
- Compliance violations related to access control requirements
- Increased likelihood of insider threat activity

---

# Severity Classification

**Severity:** High  
**Classification:** Major Exception  

**Risk Rating Rationale:**

The finding impacts access controls protecting critical systems. Former employees retaining active credentials after termination increases the likelihood of unauthorized access and creates a significant security exposure.

---

# Root Cause Analysis

## Primary Root Cause

The organization relied on a manual employee offboarding process that lacked automated communication between Human Resources and Information Technology systems.

## Contributing Factors

- HR termination records were not automatically synchronized with IAM systems.
- ServiceNow offboarding tickets were manually created and dependent on HR personnel completing an additional step.
- No automated alerting existed for overdue termination actions.
- Access review processes did not identify delayed account removal quickly enough.

---

# Corrective and Preventive Action (CAPA)

## Immediate Corrective Actions

| Action | Owner | Status |
|---|---|---|
| Disable remaining terminated user accounts | IAM Team | Completed |
| Review terminated user activity logs for unauthorized access | Security Operations | Completed |
| Document affected accounts and remediation evidence | GRC Team | Completed |

---

## Long-Term Preventive Actions

| Action | Owner | Target Date | Status |
|---|---|---|---|
| Integrate HR termination events with IAM workflows | IAM Engineering | Q4 2023 | In Progress |
| Require automated ServiceNow offboarding ticket creation | IT Operations | Q4 2023 | Planned |
| Implement automated access revocation alerts | Security Engineering | Q1 2024 | Planned |
| Perform quarterly termination access audits | GRC Team | Ongoing | Planned |

---

# Control Improvement Recommendation

Implement an automated Joiner-Mover-Leaver (JML) lifecycle management process:

1. HR initiates termination event.
2. Identity provider receives termination signal.
3. User access is automatically disabled.
4. Remaining privileged access is reviewed.
5. Evidence is captured for audit validation.

Recommended technologies/process improvements:

- Azure AD Lifecycle Workflows
- ServiceNow ITSM automation
- Identity Governance and Administration (IGA) solution
- Automated compliance reporting dashboards

---

# Validation & Evidence Requirements

The following evidence should be collected before closure:

☐ ServiceNow offboarding workflow records  
☐ Azure AD account disablement logs  
☐ GitHub access removal records  
☐ IAM audit logs  
☐ Access review reports  
☐ Updated offboarding procedures  

---

# Closure Criteria

Finding may be closed when:

- All terminated accounts are revoked within the required SLA.
- Automated workflow improvements are implemented.
- Evidence demonstrates consistent control operation.
- A follow-up audit confirms remediation effectiveness.

---

# Final Audit Assessment

**Finding Status:** Open  

The organization has identified a gap in its termination access management process. While no confirmed misuse of accounts was identified, delayed access removal creates unnecessary exposure. Implementing automated identity lifecycle controls will reduce operational dependency on manual processes and improve compliance maturity.
