# HELIX INDUSTRIES
### Windows Domain Administration Lab

A hands-on Windows Server and Active Directory administration lab built using VMware Workstation Pro on a Windows 11 laptop.

## Overview

This project simulates a small enterprise Windows domain environment to develop practical skills in Windows Server administration, Active Directory Domain Services, DNS, Group Policy, network configuration, user management and SMB file sharing.

The focus is on understanding configuration decisions, implementing services, verifying functionality and documenting troubleshooting procedures.

## Architecture

The lab runs entirely on a Lenovo laptop using Windows 11 as the host operating system and VMware Workstation as a hosted (Type 2) hypervisor.

Three virtual machines will simulate a small corporate Windows domain environment, including one Domain Controller and two domain-joined Windows workstations.

The virtual machines will communicate through a VMware virtual network, with IP addressing and DNS configured specifically for the lab.


![Helix Industries Lab Architecture](architecture/helix-architecture.png)

## Planned Virtual Machines

![Image description](screenshots/planned-vms.png)




**Active Directory Domain:** `corp.helix.test`

**NetBIOS Domain:** `HELIX`


## IP Addressing
The lab uses VMware Workstation Pro NAT networking (VMnet8), with a dedicated virtual subnet (192.168.164.0/24).

The Domain Controller (HLX-DC01) is planned to use a static IP address, while both Windows 11 clients will obtain their IP addresses through DHCP and use the Domain Controller for DNS resolution.

![Image description](docs/ip-addressing.png)

## Project Objectives

- Plan IP addressing and verify network connectivity
- Deploy a Windows Server Domain Controller
- Configure Active Directory Domain Services and DNS
- Create departmental Organizational Units, users and security groups
- Join two Windows 11 clients to the domain
- Configure and validate departmental Group Policies
- Implement SMB file sharing and mapped network drives
- Document configuration, verification and troubleshooting

## Project Status

**In Progress — Windows Client Domain Integration**
- [x] VMware Workstation available on the Lenovo laptop
- [x] Active Directory domain and VM naming planned
- [x] Configure VMware virtual networking
- [x] Validate server IP addressing and client-to-DC connectivity
- [x] Create Windows Server 2025 virtual machine
- [x] Create 2 Windows 11 virtual machines
- [x] Install Windows 11 on both clients
- [x] Configure Active Directory and DNS
- [x] Create departmental Organizational Units (IT, Engineering, Sales, Finance)
- [x] Join HLX-CL01 to corp.helix.test
- [x] Join HLX-CL02 to corp.helix.test
- [ ] Create Active Directory users and security groups
- [ ] Implement and validate Group Policies
- [ ] Configure SMB file sharing and mapped drives
- [ ] Configure and validate Windows DHCP Server
- [ ] Complete troubleshooting and final documentation

## Security and Privacy

This project uses fictitious company identities and lab-only accounts. 
