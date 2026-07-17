# Internship-Website
# Network Infrastructure Documentation Portal

## Overview

This project is a centralized documentation website developed during my internship at Beta IT. The purpose of this portal is to organize, document, and present the design, implementation, and configuration details of the enterprise network infrastructure developed in the company lab environment.

The website provides a structured reference for network architecture, VLAN design, virtual machines, firewall configuration, network services, and implementation progress throughout the project.

---

## Project Objectives

- Document the complete network infrastructure architecture.
- Maintain records of network configurations and implementation steps.
- Provide a centralized knowledge base for troubleshooting and future maintenance.
- Organize information about virtualization, networking, and security components.

---

## Infrastructure Overview

The project environment consists of:

- Cisco Layer 2 Core Switch
- FortiGate Firewall (Edge Gateway)
- ESXi Virtualization Cluster
  - ESXi Node A
  - ESXi Node B
- Virtual Machines for network services and testing
- VLAN-based network segmentation

---

## Network Segmentation

| VLAN | Purpose | Subnet |
|------|---------|--------|
| VLAN 10 | Management | 192.168.10.0/24 |
| VLAN 20 | Infrastructure Services | 192.168.20.0/24 |
| VLAN 30 | Client Devices | 192.168.30.0/24 |

---

## Implemented Services

### DNS & DHCP
Centralized network services deployed to provide hostname resolution and automatic IP address assignment.

### IP Address Management (IPAM)
NetBox was deployed to maintain centralized tracking of IP addresses, VLANs, devices, and subnet allocations.

### Jump Host
A secure Ubuntu-based Jump Host was configured to provide controlled administrative access to network devices.

### Firewall & Routing
FortiGate was implemented as the primary edge firewall responsible for:
- Inter-VLAN routing
- NAT configuration
- Security policies
- Network segmentation

---

## Virtual Machines

| VM Name | Operating System | Purpose |
|---------|------------------|---------|
| dns-dhcp-01 | Ubuntu Server | DNS & DHCP Services |
| netbox-01 | Ubuntu Server 22.04 | IPAM Management |
| bastion-01 | Ubuntu Server | Jump Host |
| win-client-01 | Windows | Client Testing |
| lin-desktop-01 | Ubuntu Desktop | Linux Client Testing |

---

## Documentation Sections

The website contains documentation for:

- Network Architecture
- VLAN Configuration
- Firewall Implementation
- Virtual Machine Deployment
- IP Addressing Scheme
- Network Testing
- Weekly Progress Reports
- Troubleshooting Notes

---

## Technologies & Tools Used

- VMware ESXi
- FortiGate Firewall
- Cisco Switching
- Ubuntu Server
- Windows Client
- NetBox IPAM
- DNS / DHCP Services
- HTML, CSS, JavaScript
- GitHub Pages

---

## Project Status

Current progress includes:

✅ Network architecture implementation  
✅ VLAN segmentation  
✅ Firewall deployment  
✅ DNS/DHCP configuration  
✅ IPAM deployment  
✅ Jump Host configuration  
✅ Client VM deployment  
✅ Documentation portal development  

Future improvements include:

- Advanced FortiGate security policies
- Backup and disaster recovery testing
- Additional monitoring solutions

---
