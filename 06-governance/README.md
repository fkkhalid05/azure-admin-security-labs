# Governance Lab

## Objective
Implement governance controls in Azure to enforce standards, manage costs, and ensure compliance across resources.

## Architecture
- Management Groups
- Azure Policy
- Policy Assignments and Initiatives
- Resource Tags
- Azure Cost Management

## Design Decisions
- Governance controls are applied centrally to reduce configuration drift
- Policies are used to enforce standards instead of manual reviews
- Tagging is used for cost allocation and ownership tracking
- Least privilege and guardrails are preferred over reactive fixes

## Steps
1. Created management group hierarchy to logically organize subscriptions.
2. Defined and assigned Azure Policies to enforce compliance requirements.
3. Used built-in policy definitions to restrict insecure configurations.
4. Applied policy assignments at management group or subscription scope.
5. Implemented resource tagging for ownership, environment, and cost tracking.
6. Reviewed compliance results and remediated non-compliant resources.
7. Used Cost Management to analyze and monitor resource spending.

## Security Considerations
- Azure Policy prevents insecure deployments before they occur
- Centralized governance reduces misconfiguration risk
- Tags improve accountability and incident response
- Cost visibility helps detect unexpected or unauthorized usage

## On-Premises Mapping
- GPO enforcement → Azure Policy
- OU structure → Management Groups
- Asset tagging → Azure resource tags
- Budget monitoring → Azure Cost Management

## Lessons Learned
- Governance should be proactive, not reactive
- Policy enforcement scales better than manual controls
- Management groups simplify large-scale administration
- Poor governance increases security and cost risk
