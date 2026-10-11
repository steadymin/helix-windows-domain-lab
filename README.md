# HELIX INDUSTRIES
### Windows Domain Administration Lab

A hands-on Windows Server and Active Directory administration lab, built on a Dell OptiPlex 7050 running Proxmox VE.

## Overview

This project simulates a small enterprise Windows domain environment to develop practical skills in Windows Server administration, Active Directory Domain Services, DNS, Group Policy, network configuration, user management and SMB file sharing.

The focus is on understanding configuration decisions, implementing services, verifying functionality and documenting troubleshooting procedures.

## Architecture

The lab uses a physical Dell OptiPlex 7050 running Proxmox VE as its virtualization host.

The host connects to the home network through an Ethernet switch and a small router operating in Client Mode, providing a wireless uplink to the main router.

A Windows 11 laptop is used as the administration workstation.

**Architecture diagram:** To be added after finalizing the network topology.

## Planned Virtual Machines

![Image description](screenshots/planned-vms.png)





**Active Directory Domain:** `corp.helix.test`

**NetBIOS Domain:** `HELIX`

## Project Objectives

- Plan IP addressing and verify network connectivity
- Deploy a Windows Server Domain Controller
- Configure Active Directory Domain Services and DNS
- Create departmental Organizational Units, users and security groups
- Join two Windows 11 clients to the domain
- Configure and validate departmental Group Policies
- Implement SMB file sharing and mapped network drives
- Document configuration, verification and troubleshooting

## Documentation

- [IP Addressing Plan](docs/ip-addressing.md)

Additional documentation and implementation evidence will be added throughout the project.

## Project Status

**In Progress — Network Discovery & Infrastructure Planning**

- [x] Proxmox VE installed on physical Dell host
- [x] Proxmox static management IP verified
- [x] Physical network topology identified
- [x] DHCP range identified
- [] Validate virtual machine network connectivity
- [ ] Deploy Windows Server and Windows clients
- [ ] Configure Active Directory and DNS
- [ ] Implement and validate Group Policies

## Security and Privacy

This project uses fictitious company identities and lab-only accounts. 