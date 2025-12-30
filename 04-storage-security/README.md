# Storage Security Lab

## Objective
Implement secure Azure storage access controls to protect data from unauthorized access and data exfiltration.

## Architecture
- Azure Storage Account
- Private Endpoints
- Azure RBAC
- Storage Account Networking
- Azure Defender for Storage

## Design Decisions
- Storage access is restricted using identity-based authentication
- Public network access is minimized to reduce exposure
- Access is granted using least privilege principles
- Monitoring and threat protection are enabled

## Steps
1. Created an Azure Storage Account with secure default settings.
2. Disabled public blob access to prevent anonymous data exposure.
3. Restricted network access using firewall rules and private endpoints.
4. Assigned RBAC roles to users and groups instead of using storage keys.
5. Enabled Microsoft Defender for Storage for threat detection.
6. Tested access to confirm least privilege enforcement.

## Security Considerations
- Avoided use of storage account access keys where possible
- Used Azure AD authentication instead of shared keys
- Limited network access to trusted sources
- Enabled monitoring to det

