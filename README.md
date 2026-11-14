# Local-Network-Port-Scanner

## Overview
This project focuses on scanning a local network to identify active devices, discover open ports, and understand the security exposure of network-connected devices using Nmap.

## Objective
- Discover active devices on a local network.
- Identify open TCP ports.
- Understand services running on different ports.
- Analyze potential security risks associated with exposed services.
- Document and save network scanning results.

## Tools Used
- Nmap – Network discovery and port scanning.
- Wireshark – Optional packet analysis.
- Windows CMD / Kali Linux Terminal.

## Scanning Methodology

### 1. Identify Local Network Range
Identified the local IP address and subnet mask to determine the network CIDR range.

### 2. Perform TCP SYN Scan
Executed the following command:

```bash
nmap -sS <network-cidr>
```

### 3. Save Scan Results
Used the following command to save the results:

```bash
nmap -sS <network-cidr> -oN scan_results.txt
```

## Results
- Identified active devices on the local network.
- Detected open TCP ports.
- Identified associated network services.
- Saved scan results for further analysis.

## Security Analysis
Open ports were examined to understand their associated services and potential security risks, including:
- Unnecessary exposed services.
- Insecure communication protocols.
- Potentially vulnerable services.
- Unnecessary remote access exposure.

## Project Structure
```text
Local-Network-Port-Scanner/
├── README.md
├── scan-results/
│   └── scan_results.txt
└── screenshots/
    └── scan_output.png
```

## Disclaimer
This project was conducted for educational purposes on an authorized local network. Always obtain permission before scanning any network.

## Learning Outcomes
- Understanding of IP addresses and CIDR notation.
- Practical experience with Nmap.
- Understanding TCP SYN scanning.
- Identifying open ports and network services.
- Basic network security assessment.
