# Network Diagram

This section contains the planned enterprise-style segmented home network architecture for the cybersecurity lab.

## Planned Networks

| Network | Subnet | Purpose |
|---|---|---|
| Home | 192.168.10.0/24 | Personal devices |
| IoT | 192.168.20.0/24 | Smart devices |
| Guest | 192.168.30.0/24 | Guest internet access |
| Work | 192.168.40.0/24 | Isolated work devices |
| Lab | 192.168.50.0/24 | Cybersecurity lab |

## Goals
- Separate IoT from personal systems
- Isolate work devices from lab traffic
- Create secure testing environment
- Practice enterprise network segmentation
- Prepare for SIEM and Active Directory deployment
