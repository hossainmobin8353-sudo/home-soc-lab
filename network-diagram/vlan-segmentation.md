# VLAN Segmentation Documentation

## Overview

This document outlines the VLAN and subnet segmentation used in the Enterprise SOC Home Lab project.

The goal of this segmentation is to isolate devices based on purpose and security level, similar to enterprise network environments.

---

# Network Architecture

```text
Internet
   |
Cox Gateway
   |
ASUS RT-BE96U Router
   |
-------------------------------------------------
|         |          |          |               |
Home    WorkNet   CyberLab    Guest          IoT
50.x      52.x      53.x       54.x          55.x
```

---

# VLAN and Subnet Configuration

| Network Name | VLAN | Subnet | Purpose |
|---|---|---|---|
| Momo_Home | Default | 192.168.50.0/24 | Personal devices |
| Momo_WorkNet | VLAN 52 | 192.168.52.0/24 | Work systems |
| Momo_CyberLab | VLAN 53 | 192.168.53.0/24 | Cybersecurity lab |
| Momo_Guest | VLAN 54 | 192.168.54.0/24 | Guest internet access |
| Momo_IoT | VLAN 55 | 192.168.55.0/24 | Smart home and IoT devices |

---

# Security Objectives

## Home Network
Used for trusted personal devices such as:
- Personal computers
- Phones
- Tablets

---

## WorkNet
Used only for:
- Work laptop
- Sensitive accounts
- Professional activity

This network is isolated from the cybersecurity lab.

---

## CyberLab
Dedicated environment for:
- VMware Workstation
- Active Directory
- Windows Server
- Kali Linux
- Splunk SIEM
- Security testing

This network is intentionally separated from production and work devices.

---

## Guest Network
Provides:
- Internet-only access
- No local network visibility
- Isolation from internal devices

---

## IoT Network
Used for:
- Smart TVs
- IoT devices
- Smart home equipment

IoT devices are isolated to reduce security risks and prevent lateral movement.

---

# Skills Demonstrated

This project demonstrates:
- VLAN segmentation
- Enterprise wireless architecture
- Network isolation
- Cybersecurity infrastructure planning
- Secure network design
- Subnetting
- ASUS enterprise-style router configuration

---

# Future Expansion

Planned additions:
- Active Directory deployment
- Windows domain environment
- Splunk SIEM integration
- Sysmon logging
- Vulnerability scanning
- SOC alert monitoring
- Incident response simulations
