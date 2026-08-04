# Mock Audit Finding Report
**Audit Type:** Internal Security & Access Control Audit  
**Framework Alignment:** NIST SP 800-53 / ISO 27001 / SOC 2 Access Management Principles  

# Audit Finding: DEL-2023-01

## Finding ID

**DEL-2023-01**

## Title

**Delayed User Offboarding**

## Severity

**High**

## Failed Control

**AC-02 - Account Management (Terminated User Revocation)**

---

## Observation

During the review of Q2 employee terminations, auditors sampled **15 departed employees** to evaluate compliance with the organization's user access termination procedures.

The audit identified that **3 out of 15 terminated employees** did not have their Azure Active Directory and GitHub access revoked within the required **24-hour SLA**.

Access remained active for an average of **9 days after termination**, indicating that the offboarding process was not consistently executed within required timelines.

---

## Risk

Delayed removal of user access increases the likelihood of unauthorized access to organizational systems after employment termination.

Potential impacts include:

- Unauthorized access to proprietary source code
- Exposure of sensitive organizational data
- Unauthorized changes to production environments
- Increased insider threat risk
- Potential non-compliance with security and access control requirements

---

## Root Cause

The termination process relied on manual coordination between Human Resources and Information Technology.

HR completed employee termination actions within the payroll system but did not consistently trigger the required ServiceNow offboarding workflow for IT.

Contributing factors included:

- Lack of automated HR-to-IAM integration
- Manual dependency for ticket creation
- Limited monitoring of termination SLA compliance

---

## Recommendation

Implement an automated Joiner-Mover-Leaver (JML) process to improve termination access management.

Recommended actions:

1. Integrate HR termination events with identity management systems.
2. Automatically generate ServiceNow offboarding tickets upon termination.
3. Implement automated alerts for overdue access removal activities.
4. Perform periodic access reviews to validate termination control effectiveness.

---

## Management Response

Management agrees with the finding and recognizes the risk associated with delayed user access removal.

The organization will implement automated offboarding workflows between HR, ServiceNow, and identity management platforms to reduce manual errors and improve compliance with the 24-hour termination SLA.

Planned remediation activities include:

- IAM workflow automation
- Updated termination procedures
- Quarterly termination access audits
- Evidence collection improvements for future audits

---

## Corrective Action Plan (CAPA)

| Action Item | Owner | Target Date | Status |
|---|---|---|---|
| Disable remaining inactive terminated accounts | IAM Team | Completed | Closed |
| Automate HR termination notifications | IAM Engineering | Q4 2023 | In Progress |
| Configure SLA monitoring alerts | Security Operations | Q1 2024 | Planned |
| Update offboarding procedures | GRC Team | Q1 2024 | Planned |

---

## Evidence Required for Closure

- Azure AD account disablement logs
- GitHub access removal records
- ServiceNow offboarding tickets
- Updated termination procedures
- Access review reports

---

## Finding Status

**Open - Remediation In Progress**
