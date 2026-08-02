## Compliance Scope

Defining boundaries is the most critical first step of any audit. If we do not scope correctly, auditors may examine systems that do not impact customer data, increasing audit effort and creating unnecessary findings.

| **Category** | **In Scope** | **Out of Scope** |
|--------------|--------------|------------------|
| **Environments** | Azure Production Tenant<br>Azure Disaster Recovery (DR) Environment | Lab/Sandbox Environments<br>Marketing Website |
| **Assets / Endpoints** | Admin Workstations<br>Production Servers | Standard Corporate Laptops (Non-Admins) |
| **Data** | Customer Backup Data<br>Protected Health Information (PHI)<br>Cardholder Data (PCI) | Internal HR/Payroll Data<br>Marketing Analytics |
| **Identity** | Microsoft Entra ID (Production & Corporate) | Legacy Active Directory (Decommissioned) |
| **Processes** | Change Management<br>Incident Response<br>Backup & Recovery | Marketing Campaigns<br>Standard HR Onboarding |
| **Vendors** | Microsoft Azure<br>CrowdStrike<br>GitHub Enterprise | HR Payroll Vendor<br>Catering Services |
