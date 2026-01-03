# Secure Multi-Branch Enterprise WAN (Cisco Packet Tracer)

## Overview
This project simulates a **real-world enterprise WAN architecture** for a banking environment using **Cisco Packet Tracer**.

The objective is to move beyond CCNA theory and design a **secure, scalable, and well-documented enterprise network** that reflects how production networks are built.

The topology follows a **hub-and-spoke WAN model** with a central HQ and five branch offices.

---
## Topology Overview
- 1 Headquarters (HQ)
- 5 Branch Offices
- Hub-and-spoke WAN design
- Dedicated ISP router

---

## Technologies Implemented
- OSPF (single area) with MD5 authentication
- VLAN segmentation (router-on-a-stick)
- NAT (PAT) for Internet access
- Extended ACLs for inter-branch traffic restriction
- SSH-only device management
- Network hardening best practices
- ISP simulation
---

## Addressing & Segmentation
- Each branch uses VLANs 10, 20, and 30
- Inter-branch traffic is restricted by ACLs
- Only approved networks can reach HQ resources
---

## Technologies Used
- Cisco 2911 Routers
- Cisco 2960 Switches
- Cisco Packet Tracer
- OSPF (Area 0)
- VLANs & 802.1Q
- NAT Overload (PAT)
- Extended ACLs
- SSH, CDP hardening

---

## Repository Structure
- `packet-tracer/` – Packet Tracer topology files
- `configs/` – Full device configurations
- `security/` – ACLs and security policy documentation
- `routing/` – OSPF design and authentication
- `nat/` – NAT configuration and explanation
- `verification/` – Testing and validation steps
- `future-work/` – Planned improvements (IPSec, redundancy, GNS3)

---

## Verification & Testing

- Verified OSPF neighbor relationships between HQ and all branch routers
- Confirmed end-to-end IP connectivity using ICMP (ping)
- Validated VLAN segmentation and inter-VLAN routing
- Tested NAT translation at the WAN edge
- Confirmed SSH-only remote access to network devices
- Verified ACL enforcement between network segments

---
## Packet Tracer Simulation File

📁 **Topology File:**  
[Download Banking-WAN-HQ-Branches.pkt](Banking-WAN-HQ-Branches.pkt)

> Open using Cisco Packet Tracer (version 8.x or later).

## Future Enhancements
- IPSec Site-to-Site VPNs
- Redundancy (HSRP)
- Dual ISP failover
- Migration to GNS3 for advanced features

---

## Author
**Odera Gerald Akwaeze**  
Networking | Security | Enterprise WAN Design


