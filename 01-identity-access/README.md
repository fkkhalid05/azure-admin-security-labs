# Identity and Access Management Lab

## Objective
Implement secure identity and access management using Azure Entra ID.

## Architecture
- Azure Entra ID
- Users and Groups
- RBAC
- Conditional Access

## Steps
1. Created users and security groups
2. Assigned RBAC roles at resource group scope
3. Enabled MFA for admin accounts
4. Tested least privilege access

## Security Considerations
- Enforced MFA for privileged users
- Applied least privilege access
- Avoided use of Global Administrator

## On-Premises Mapping
- Active Directory → Azure Entra ID
- Group Policy → Conditional Access

## Lessons Learned
- RBAC scope selection is critical
- Identity misconfiguration is a major attack vector

