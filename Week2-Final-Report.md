# Cybersecurity Practical Labs — Week 2 Final Report

**Training Program:** NetworkWalks Cybersecurity Internship  
**Participant:** James Kwabena Incoom  
**Week:** 2  
**Project:** Network Discovery, Host Identification and Open-Source Intelligence (OSINT)

---

## 1. Introduction

This report documents the practical cybersecurity exercises completed during Week 2 of my NetworkWalks cybersecurity training.

The exercises focused on network discovery, host identification, network topology visualization and open-source intelligence gathering.

The practical activities were performed using Parrot Security OS in a VMware virtual environment.

## 2. Lab Environment

The following technologies were used:

- VMware Workstation
- Parrot Security OS
- Nmap
- Zenmap
- theHarvester
- Windows Server 2022 lab environment
- VMware virtual networking

**Network tested:** 192.168.32.0/24  
**Target IP tested:** 192.168.32.50  
**Observed default gateway:** 192.168.32.2

All active network discovery activities were conducted within my virtual lab environment.

## 3. Lab 1 — Network Discovery Using Nmap

### Objective

Identify active hosts within the virtual network and examine the results of network discovery.

### Commands Used

```bash
ping -c 4 192.168.32.50
```

```bash
sudo nmap -sn 192.168.32.0/24
```

### Results

The network discovery exercise produced the following observations:

1. Six active IP addresses were identified within the virtual network.
2. VMware MAC addresses were identified for five discovered hosts.
3. ICMP connectivity to 192.168.32.50 was confirmed.
4. The scan helped identify reachable devices within the VMware network.

### Technical Explanation

Nmap is a network scanning tool used for host discovery, service identification and security assessment.

The `-sn` option performs host discovery without a port scan.

The `sudo` command provides elevated privileges, allowing Nmap to use additional discovery methods where supported.

### Troubleshooting Observation

During the initial discovery process, Zenmap did not display all the expected hosts.

After performing the discovery using elevated privileges, additional hosts were identified.

This demonstrated the importance of understanding how permissions and discovery methods can affect network scanning results.

## 4. Lab 2 — Network Topology Visualization Using Zenmap

### Objective

Visualize discovered network devices and understand their relationships within the virtual network.

### Activities

1. Opened Zenmap.
2. Configured the network discovery scan.
3. Executed the scan against the virtual network.
4. Reviewed discovered hosts.
5. Examined the topology visualization.
6. Captured screenshots of the results.

### Results

Zenmap provided a graphical representation of the network discovery results.

The exercise helped me understand how network discovery information can support network documentation and troubleshooting.

### Evidence

- `networkwalks_Zenmap_Teopology.png`
- `Scan_sever2022_.png`

## 5. Lab 3 — Open-Source Intelligence Using theHarvester

### Objective

Understand how publicly available information can be collected during passive reconnaissance.

### Activities

1. Verified theHarvester installation.
2. Reviewed its command-line options.
3. Conducted an OSINT search for `networkwalks.com`.
4. Selected the CRTsh information source.
5. Reviewed the returned results.

### Results

The search returned:

- IP addresses: None found
- Email addresses: None found
- People: None found
- Hosts: None found

### Technical Explanation

theHarvester is an open-source intelligence tool that collects publicly available information from supported data sources.

Unlike Nmap, theHarvester does not perform local network host discovery through ARP scanning.

Therefore, the absence of results from theHarvester does not indicate that devices are missing from the local network.

The results indicate that the selected information source did not return matching information during this particular search.

### Evidence

- `theHarvester_installed.png`
- `networkwalks.com_scan_.png`

## 6. Challenges and Troubleshooting

### Challenge 1 — Incomplete Host Discovery

**Problem:** The initial network discovery did not display all expected hosts.

**Action:** Repeated the discovery using elevated privileges.

**Outcome:** Additional hosts were identified.

**Lesson learned:** Network discovery results can depend on permissions, scanning techniques and network configuration.

### Challenge 2 — No OSINT Results

**Problem:** theHarvester returned no matching information for the selected target.

**Action:** Reviewed the tool's output and available search options.

**Outcome:** Confirmed that the selected search source returned no IP addresses, email addresses, people or hosts.

**Lesson learned:** Different reconnaissance tools use different information sources and techniques.

### Challenge 3 — Organizing Lab Evidence

**Problem:** Screenshots needed to be transferred from Parrot Security OS to Windows for documentation.

**Action:** Used a VMware shared folder to transfer screenshots to the Windows host.

**Outcome:** Successfully organized the screenshots and uploaded the relevant evidence to GitHub.

## 7. Skills Practiced

- Linux command-line operations
- Network discovery using Nmap
- ICMP connectivity testing
- IP address identification
- MAC address identification
- Network topology visualization
- Basic reconnaissance techniques
- Open-source intelligence gathering
- Troubleshooting network discovery
- Technical documentation
- GitHub portfolio management

## 8. Conclusion

The Week 2 practical exercises improved my understanding of network discovery and open-source intelligence gathering.

Using Nmap and Zenmap, I practiced identifying active devices and examining network topology within my VMware lab.

Using theHarvester, I explored how publicly available information can be collected during reconnaissance.

The exercises also helped me develop troubleshooting, documentation and evidence-management skills.

## 9. Future Practical Work

My next planned lab will focus on further investigating host discovery and comparing network scanning results with local ARP and DNS information.

I also plan to examine the differences between internal DNS discovery and public OSINT reconnaissance.

**Project Status:** Week 2 practical exercises documented.

**GitHub Repository:** Cybersecurity-labs-week2
## 10. Week 2 Assessment Results

**Training:** NetworkWalks Cybersecurity Internship
**Batch:** B084
**Assessment status:** Marked
**Final score:** 100/100 (100%)

| Assessment criterion | Score |
| --- | ---: |
| Timely submission | 10/10 |
| GitHub repository | 40/40 |
| LinkedIn project post | 40/40 |
| YouTube experience sharing | 10/10 |
| **Total** | **100/100** |

The NetworkWalks results portal confirmed full marks for my Week 2 practical assignment. This result reflects my weekly internship project assessment, not a separate professional certification.
