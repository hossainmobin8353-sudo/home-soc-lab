# Planned Home SOC Lab Topology

## Current Hardware
- Cox WiFi 7 Gateway
- ASUS BE19000 Router
- VMware Host System

---

# Planned Segmentation

## HOME NETWORK
Purpose:
- Personal devices
- Phones
- Tablets

Subnet:
192.168.10.0/24

---

## IOT NETWORK
Purpose:
- Smart TVs
- Smart home devices
- Printers

Subnet:
192.168.20.0/24

Restrictions:
- No access to Home or Work networks

---

## GUEST NETWORK
Purpose:
- Guest WiFi access

Subnet:
192.168.30.0/24

Restrictions:
- Internet only

---

## WORK NETWORK
Purpose:
- Work laptop
- Secure work devices

Subnet:
192.168.40.0/24

Restrictions:
- Isolated from Lab and IoT networks

---

## CYBER LAB NETWORK
Purpose:
- VMware lab environment
- Active Directory
- Kali Linux
- Splunk SIEM

Subnet:
192.168.50.0/24

Restrictions:
- Controlled access
- Isolated from Work devices

---

# Planned Lab Systems

| System | Role |
|---|---|
| Windows Server | Active Directory Domain Controller |
| Windows 11 | Domain workstation |
| Kali Linux | Security testing |
| Splunk | SIEM and log analysis |

---

# Security Goals
- Practice enterprise network segmentation
- Isolate insecure IoT devices
- Build safe cybersecurity testing environment
- Simulate enterprise Active Directory infrastructure
- Gain hands-on SOC analyst experience
