# Identity and Access Management Lab

## Objective
Implement secure identity and access management using Azure Entra ID.

## Architecture
- Azure Entra ID
- Users and Groups
- RBAC
- Conditional Access

## Steps
1. created separate admin and reader users in azure Entra ID to model privileged and low privileged identities
2. Created security groups to represent administrator and read-only roles. Users were added to groups so permissions can be managed centrally.
3. Assigned RBAC roles to security groups at resource group scope to enforce least privilege access.

4. Enabled MFA for admin accounts: Enforced MFA for privileged admin accounts to reduce the risk of credential compromise.
5. Tested least privilege access

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

