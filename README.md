# Cybersecurity Practical Labs — Week 2

## Project Overview
This repository documents my hands-on cybersecurity training using Parrot Security OS, Nmap, Zenmap, and theHarvester.

The objective is to develop practical skills in network discovery, host identification, MAC address discovery, and open-source intelligence (OSINT).

## Lab Environment
- VMware Workstation
- Parrot Security OS
- Nmap and Zenmap
- theHarvester
- Windows Server 2022 lab
- VMware virtual network

## Lab 1: Network Discovery with Nmap and Zenmap

**Objective:** Identify active devices on my virtual network and visualize the discovered hosts.

**Commands used:**
```bash
ping -c 4 192.168.32.50
sudo nmap -sn 192.168.32.0/24
```

**Results:**
- Discovered six active IP addresses in the virtual network.
- Identified VMware MAC addresses for five discovered hosts.
- Confirmed ICMP connectivity to 192.168.32.50.
- Generated a network topology visualization using Zenmap.

**Evidence:**
- `networkwalks_Zenmap_Teopology.png`
- `Scan_sever2022_.png`

## Lab 2: Open-Source Intelligence with theHarvester

**Objective:** Learn how publicly available information can be collected during reconnaissance.

**Activities:**
- Verified theHarvester installation.
- Explored its command-line options.
- Performed an OSINT search for networkwalks.com using the CRTsh source.

**Results:**
The search returned no IP addresses, email addresses, people, or hosts. This demonstrates that an OSINT search may return no results from a particular source.

**Evidence:**
- `theHarvester_installed.png`
- `networkwalks.com_scan_.png`

## Skills Practiced
- Network discovery
- ICMP connectivity testing
- MAC address identification
- Network topology visualization
- Linux command-line operations
- OSINT reconnaissance
- Technical documentation

## Conclusion
These practical exercises helped me understand how network discovery and passive reconnaissance tools operate. All active network scanning was performed within my own virtual lab environment.
