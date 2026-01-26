# Network Security Lab

## Objective
Design and secure an Azure virtual network using Network Security
Groups (NSGs) and least-privilege network access controls.

---

## Architecture
- Virtual Network (VNet)
- Single subnet (default)
- Network Security Group (NSG) associated at subnet level

---

## Steps

1. Created an Azure Virtual Network with a defined address space
   and a default subnet.

2. Created a Network Security Group (NSG) in the same resource group
   and region as the virtual network.

3. Configured inbound NSG rules to allow SSH (TCP 22) access only
   from a trusted public IP address using CIDR notation (/32).

4. Verified default NSG rules to confirm a secure deny-by-default
   inbound posture.

5. Associated the NSG with the subnet to enforce network security
   for all resources deployed within the subnet.

---

## Security Considerations
- Implemented least-privilege network access
- Restricted inbound access to a single trusted IP
- Maintained default deny inbound rules
- Applied NSG at subnet level for centralized control

---

## On-Premises Mapping
- VLANs → Azure Subnets
- Firewalls → Network Security Groups
- Network segmentation → Zero Trust networking principles

---

## Lessons Learned
- NSG rule priority determines traffic flow
- Default NSG rules provide a secure baseline
- NSGs must be associated with a subnet or NIC to be effective
- Valid CIDR notation is required for NSG rule configuration
