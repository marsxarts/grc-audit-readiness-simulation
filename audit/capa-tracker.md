# Corrective and Preventive Action (CAPA) Tracker

## Overview

**Purpose:**  
This tracker documents the corrective and preventive actions taken to address audit findings and ensure identified control weaknesses are remediated effectively.


---

# CAPA Summary

| Finding ID | Finding Title | Severity | Overall Status |
|---|---|---|---|
| DEL-2023-01 | Delayed User Offboarding | High | Remediation In Progress |

---

# Corrective Action Details

## Finding ID: DEL-2023-01

**Finding:** Delayed User Offboarding  
**Failed Control:** AC-02 - Account Management  
**Risk Area:** Identity and Access Management (IAM)

---

## Remediation Actions

| Action ID | Corrective / Preventive Action | Owner | Due Date | Priority | Status |
|---|---|---|---|---|---|
| CAPA-001 | Immediately revoke the 3 active terminated user accounts identified during audit testing. | IT Administrator | Oct 25, 2023 | High |  Closed |
| CAPA-002 | Integrate HR system with Entra ID through API automation to disable accounts when termination status changes. | IT / HR Teams | Nov 15, 2023 | High |  In Progress |
| CAPA-003 | Update employee offboarding policy and procedures to reflect the automated termination workflow. | GRC Team | Nov 20, 2023 | Medium |  Not Started |

---

# Action Item Details

## CAPA-001: Immediate Account Revocation

**Objective:**  
Remove unauthorized access exposure by disabling all terminated user accounts identified during audit testing.

**Completed Activities:**

- Disabled 3 terminated user accounts.
- Removed Azure Active Directory access.
- Removed GitHub repository permissions.
- Reviewed account activity logs.

**Validation Evidence:**

- Azure Entra ID disablement logs
- GitHub access removal records
- IT ticket completion records

**Status:** Closed

---

## CAPA-002: Automated Account Disablement

**Objective:**  
Reduce dependency on manual processes by integrating HR termination events with identity management systems.

**Planned Activities:**

- Configure HR system termination triggers.
- Create automated workflow between HR platform and Entra ID.
- Automatically disable user accounts when termination status changes.
- Generate audit logs for verification.

**Success Criteria:**

- Terminated accounts disabled within the required 24-hour SLA.
- Automated workflow generates traceable evidence.
- Manual ticket creation is no longer required.

**Owner:** IT / HR Teams  
**Target Completion:** November 15, 2023  
**Status:** In Progress

---

## CAPA-003: Offboarding Policy Update

**Objective:**  
Ensure organizational procedures accurately reflect the updated automated offboarding process.

**Planned Activities:**

- Update employee termination procedures.
- Define roles and responsibilities between HR, IT, and Security.
- Document escalation procedures for failed automation events.

**Success Criteria:**

- Updated policy approved.
- Stakeholders trained on revised process.
- Policy version documented for future audits.

**Owner:** GRC Team  
**Target Completion:** November 20, 2023  
**Status:** Not Started

---

# Closure Requirements

Finding DEL-2023-01 can be closed when:

- ✅ All identified terminated accounts have been revoked.
- ☐ Automated HR-to-Entra ID workflow is operational.
- ☐ Offboarding policy updates are approved.
- ☐ Evidence demonstrates the control is operating effectively.
- ☐ Follow-up testing confirms compliance with the 24-hour SLA.

---

# Final CAPA Status

**Current Status:** Remediation In Progress

**Next Review Date:** After completion of automation implementation

**Risk Reduction Expected:**  
Automation of identity lifecycle processes will reduce manual errors, improve termination response times, and strengthen compliance with access control requirements.
