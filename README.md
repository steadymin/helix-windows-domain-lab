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


**Architecture diagram:** ![Helix Industries Lab Architecture](architecture/helix-architecture.png)

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

**In Progress — VMware Infrastructure Planning**

- [x] VMware Workstation available on the Lenovo laptop
- [x] Active Directory domain and VM naming planned
- []  Configure VMware virtual networking
- []  Validate IP addressing and connectivity
- []  Create Windows Server 2025 virtual machine
- []  Create 2 Windows 11 virtual machines
- []  Configure Active Directory and DNS
- []  Implement and validate Group Policies

## Security and Privacy

This project uses fictitious company identities and lab-only accounts. 