# Network Security Lab

## Objective
Design and secure Azure virtual networks using network security controls.

## Architecture
- Virtual Network (VNET)
- Subnets
- Network Security Groups (NSGs)
- Private Endpoints

## Steps
1. Created a virtual network with multiple subnets :Created a virtual network with segmented subnets to isolate workloads.
2. Applied Network Security Groups to subnets : Associated a Network Security Group with the web subnet.
3. Defined inbound and outbound security rules : Implemented inbound NSG rules to allow only required traffic.
4. Tested traffic flow between subnets
5. Restricted public access where possible

## Security Considerations
- Implemented least privilege network access
- Restricted unnecessary inbound ports
- Segmented workloads using subnets

## On-Premises Mapping
- VLANs → Azure Subnets
- Firewalls → NSGs
- Network segmentation → Zero Trust networking

## Lessons Learned
- NSG rule priority is critical
- Default rules should not be blindly trusted
