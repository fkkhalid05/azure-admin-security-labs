
# Virtual Machine Security Lab

## Objective
Deploy and secure Azure virtual machines following security best practices.

## Architecture
- Azure Virtual Machines
- Network Security Groups
- Azure Bastion
- Microsoft Defender for Cloud

## Steps
1. Deployed a Windows/Linux virtual machine
2. Removed public IP exposure
3. Configured NSG rules to restrict inbound access
4. Accessed VM securely using Azure Bastion
5. Enabled Microsoft Defender for Cloud

## Security Considerations
- Avoided exposing VMs directly to the internet
- Applied least privilege network access
- Used secure access methods instead of RDP/SSH over public IP

## On-Premises Mapping
- Physical servers → Azure VMs
- Jump servers → Azure Bastion
- Host hardening → VM security configuration

## Lessons Learned
- Public IPs significantly increase attack surface
- Bastion improves security posture with minimal overhead
