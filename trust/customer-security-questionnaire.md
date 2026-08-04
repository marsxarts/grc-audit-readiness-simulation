# Customer Trust & Security Questionnaire

## Purpose

Enterprise customers routinely perform security due diligence before signing contracts with SaaS providers. The purpose of this questionnaire is to demonstrate NimbusVault's security posture and provide evidence supporting key security controls.

> **Scenario:** A prospective healthcare customer has requested security documentation as part of their third-party risk assessment prior to contract execution.

---

## Security Questionnaire

| Question | Response | Supporting Evidence |
|----------|----------|---------------------|
| Do you enforce Multi-Factor Authentication (MFA) for all privileged and remote access accounts? | Yes | Access Control Policy, Microsoft Entra ID MFA Configuration Export (EVD-004) |
| Is customer data encrypted at rest? | Yes | Azure Storage Encryption (AES-256), Data Classification & Handling Policy |
| Is customer data encrypted in transit? | Yes | TLS 1.2+ enforced for all external communications. |
| Do you perform quarterly logical access reviews? | Yes | Q3 Access Review Report (EVD-001) |
| Are terminated employee accounts disabled within a defined SLA? | Yes. Accounts are disabled within 24 hours according to policy. Exceptions are tracked through CAPA. | Account Deprovisioning Report (EVD-003) |
| Are production backups performed regularly? | Yes | Azure Backup Job Summary (EVD-005) |
| Are backup restorations tested? | Yes. Monthly restoration testing is performed. | Monthly Backup Restore Test Report (EVD-006) |
| Do you conduct vulnerability scanning? | Yes. External-facing assets are scanned monthly and critical vulnerabilities are remediated according to policy. | September Vulnerability Scan Report (EVD-008) |
| Do you perform independent penetration testing? | Yes. An independent third party performs annual penetration testing. | Annual Third-Party Penetration Test Report (EVD-009) |
| Do you maintain a documented Incident Response Plan? | Yes | Incident Response Plan (EVD-012) |
| Is the Incident Response Plan tested? | Yes. Tabletop exercises are conducted annually. | Tabletop Exercise Report (EVD-013) |
| Do you maintain centralized security logging and monitoring? | Yes | SIEM Monitoring Dashboard (EVD-015) |
| Do you conduct annual security awareness training? | Yes | Annual Security Awareness Training Report (EVD-019) |
| Do you assess critical third-party vendors? | Yes. Annual vendor security assessments are performed. | Vendor Risk Assessment (EVD-018) |
| Are critical cloud providers independently audited? | Yes. NimbusVault reviews Microsoft's SOC 2 Type II, ISO 27001 certification, and FedRAMP authorization annually. | Vendor Assessment Documentation |
| Do you maintain Business Continuity and Disaster Recovery plans? | Yes | Disaster Recovery Exercise Report (EVD-007) |
| Can you provide your latest SOC 2 Type II Report? | Available upon execution of a Non-Disclosure Agreement (NDA). | Customer Trust Portal / GRC Team |
| Do you process Protected Health Information (PHI)? | Yes. Appropriate administrative, technical, and physical safeguards are implemented in accordance with HIPAA requirements. | HIPAA Control Matrix |
| Do you have a formal Vendor Risk Management Program? | Yes | Vendor Risk Management Policy |
| How are security findings tracked and remediated? | Findings are documented, risk-rated, assigned owners, and tracked through a formal Corrective and Preventive Action (CAPA) process. | Audit Findings Register & CAPA Tracker |

---

## Standard Documentation Available Upon Request

- SOC 2 Type II Report (under NDA)
- ISO 27001 Certificate
- Security Whitepaper
- Incident Response Summary
- Business Continuity Overview
- Vendor Risk Assessment Summary
- Penetration Test Attestation
- Security Awareness Program Overview

---

## Customer Assurance Statement

NimbusVault maintains a risk-based Governance, Risk, and Compliance (GRC) program designed to protect customer information, satisfy regulatory obligations, and continuously improve security operations. Evidence supporting security controls is maintained in a centralized evidence repository and is available to qualified customers under appropriate confidentiality agreements.
