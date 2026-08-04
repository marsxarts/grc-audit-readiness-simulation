# Vendor Risk Assessment (TPRM)

## Vendor Profile

- **Vendor:** Microsoft Azure
- **Service Provided:** Cloud Infrastructure / Data Hosting
- **Inherent Risk:** 🔴 **Critical** *(Hosts all customer backup data)*

## Document & Artifact Review

| Artifact Reviewed | Date Reviewed | Status / Findings | Resulting Action |
| :--- | :---: | :--- | :--- |
| **Azure SOC 2 Type II Report** | Oct 10, 2023 | Clean opinion. No exceptions noted in physical security or network controls. | Rely on Microsoft's physical controls. |
| **Azure ISO 27001 Cert** | Oct 10, 2023 | Valid through 2025. | Satisfies ISO vendor requirement. |
| **Azure FedRAMP High Auth** | Oct 10, 2023 | Authorized. | Allows us to pursue FedRAMP for Gov clients. |
| **Shared Responsibility Model** | Oct 12, 2023 | Microsoft secures the cloud; NimbusVault secures what is in the cloud. | Update internal matrix to reflect inherited vs. internal controls. |

## Assessment Outcome

- **Residual Risk Rating:** 🟢 **Low** *(Due to Microsoft's mature, independently audited security posture).*

