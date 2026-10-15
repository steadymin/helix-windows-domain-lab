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

**In Progress — Group Policy Implementation**

### Infrastructure & Networking
- [x] Set up VMware Workstation Pro
- [x] Configure VMware NAT networking (VMnet8)
- [x] Deploy Windows Server 2025 (HLX-DC01)
- [x] Deploy two Windows 11 Pro clients
- [x] Configure static IP addressing and DNS
- [x] Join both Windows 11 clients to corp.helix.test

### Active Directory
- [x] Install and configure AD DS and DNS
- [x] Create Active Directory forest and domain
- [x] Create departmental Organizational Units
- [x] Create domain users and Global Security Groups
- [x] Validate domain user authentication

### Group Policy
- [x] Deploy and validate Engineering wallpaper GPO
- [x] Configure USB storage restrictions for non-IT departments
- [x] Validate USB restrictions on HLX-CL01
- [x] Validate USB restrictions on HLX-CL02
- [ ] Validate IT workstation exception
- [ ] Configure Sales mapped drive GPO
- [ ] Configure Adobe Acrobat AI restriction GPO

### File Services
- [ ] Configure SMB file sharing
- [ ] Configure NTFS and share permissions
- [ ] Validate mapped drives and access permissions

### DHCP Server
- [ ] Install and authorize Windows DHCP Server
- [ ] Configure DHCP scope and options
- [ ] Validate DHCP leases on Windows 11 clients

### Final Validation & Documentation
- [ ] Complete Group Policy testing
- [ ] Document troubleshooting scenarios
- [ ] Finalize GitHub documentation and evidence



## Security and Privacy

This project uses fictitious company identities and lab-only accounts. 
