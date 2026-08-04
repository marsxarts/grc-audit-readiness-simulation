# Third-Party Risk Assessment (TPRM)

## Purpose

NimbusVault relies on third-party service providers to support critical business operations and customer services. This assessment documents the security review performed on Microsoft Azure, validates inherited cloud security controls, and evaluates the residual risk associated with using Azure as NimbusVault's primary cloud hosting provider.

---

# Vendor Profile

| **Attribute** | **Value** |
|---------------|-----------|
| **Vendor** | Microsoft Azure |
| **Service Provided** | Cloud Infrastructure / Data Hosting |
| **Business Owner** | Director of Cloud Operations |
| **Assessment Owner** | GRC Manager |
| **Vendor Criticality** | 🔴 Critical |
| **Inherent Risk** | 🔴 Critical |
| **Review Frequency** | Annual |
| **Assessment Date** | October 12, 2023 |
| **Next Review Date** | October 2024 |

---

# Business Justification

Microsoft Azure hosts NimbusVault's production workloads, customer backup data, disaster recovery environment, and identity infrastructure. Because Azure supports critical business services and customer data, the vendor is classified as a **Critical Third-Party Provider** requiring annual security assessments.

---

# Security Documentation Review

| **Artifact Reviewed** | **Date Reviewed** | **Status / Findings** | **Resulting Action** |
|------------------------|:-----------------:|-----------------------|----------------------|
| Azure SOC 2 Type II Report | Oct 10, 2023 | Clean audit opinion with no exceptions affecting inherited physical or infrastructure security controls. | Accept inherited physical security controls. |
| Azure ISO 27001 Certificate | Oct 10, 2023 | Certification verified and valid through 2025. | Satisfies ISO 27001 third-party assurance requirements. |
| Azure FedRAMP High Authorization | Oct 10, 2023 | Active FedRAMP High Authorization confirmed. | Supports NimbusVault's FedRAMP compliance objectives. |
| Microsoft Shared Responsibility Model | Oct 12, 2023 | Clearly defines Microsoft's infrastructure responsibilities versus NimbusVault's customer responsibilities. | Update internal control mappings to distinguish inherited and customer-managed controls. |

---

# Inherited Controls

NimbusVault relies on Microsoft Azure's independently audited security program for the following inherited controls.

| **NimbusVault Control** | **Inherited Vendor Support** |
|-------------------------|------------------------------|
| BC-01 | Azure Backup Infrastructure |
| BC-02 | Azure Disaster Recovery Infrastructure |
| LM-01 | Azure Monitor & Log Management Services |
| VR-01 | Microsoft SOC 2 Type II & ISO 27001 Assurance Reports |
| CR-01 | Azure Availability Zones & Regional Resiliency |

---

# Shared Responsibility Model

Microsoft Azure is responsible for securing the underlying cloud infrastructure, including:

- Physical data center security
- Environmental controls
- Network infrastructure
- Hypervisor security
- Hardware lifecycle management
- Global cloud availability

NimbusVault remains responsible for:

- Identity and Access Management (Microsoft Entra ID)
- Customer account provisioning and deprovisioning
- Data classification and retention
- Customer data encryption configuration
- Vulnerability management
- Application security
- Security monitoring
- Incident response
- Compliance documentation
- Customer security questionnaires

---

# Residual Risks

Although Microsoft Azure maintains a mature security program, NimbusVault retains responsibility for several customer-managed risks.

| **Residual Risk** | **Mitigation** |
|-------------------|----------------|
| Misconfigured cloud resources | Infrastructure reviews and change management |
| Excessive privileged access | Quarterly access reviews (AC-01) |
| Customer data exposure | Encryption, access controls, and monitoring |
| Application vulnerabilities | Monthly vulnerability scanning and patch management |
| Identity compromise | Multi-Factor Authentication and Conditional Access |

---

# Assessment Outcome

| **Category** | **Result** |
|--------------|------------|
| Overall Vendor Rating | ✅ Approved |
| Vendor Criticality | 🔴 Critical |
| Residual Risk | 🟢 Low |
| Executive Approval | GRC Manager |

Microsoft Azure maintains a mature security and compliance program supported by independent third-party audits and globally recognized certifications. Based on the evidence reviewed, NimbusVault will continue to rely on Azure's inherited controls while maintaining responsibility for customer-managed controls under the Shared Responsibility Model.

No significant deficiencies were identified during this assessment.

---

# Related Governance Artifacts

This assessment supports the following compliance documentation within the NimbusVault GRC Program:

- Unified Control Matrix
- Enterprise Risk Register
- Evidence Register
- Customer Security Questionnaire
- Executive Dashboard
