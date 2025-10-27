# Task 5: Analyze Network Traffic Using Wireshark
Name: Krushal Hirpara
Date: 27 October 2025

================================================================================

SUBMISSION FILES

1. README.md - This file
2. report.txt - Complete analysis with step-by-step process and findings
3. notes.txt - Theory and concepts learned during this task
4. Capture.pcapng - Packet capture file (547 packets, 124.4 KB)

================================================================================

TASK SUMMARY

Captured live network traffic using Wireshark for 2 minutes (123.8 seconds)

Total Packets: 547 packets (124.4 KB)
Interface: wlan0 (WiFi)
Duration: 2 minutes 4 seconds

Protocols Identified: 10+

Main Protocols Found:
- TCP (401 packets, 73.3%) - Connection-oriented traffic
- TLS/SSL (116 packets, 21.2%) - Encrypted HTTPS
- DNS (30 packets, 5.5%) - Domain lookups
- ICMPv6 (45 packets, 8.2%) - IPv6 diagnostics
- QUIC (26 packets, 4.8%) - Modern transport protocol
- ICMP (11 packets, 2.0%) - Ping
- ARP (10 packets, 1.8%) - Address resolution
- NTP (4 packets, 0.7%) - Time sync
- HTTP (2 packets, 0.4%) - Web requests
- mDNS (2 packets, 0.4%) - Service discovery

================================================================================

WEBSITES ACCESSED

Successfully resolved and connected to:
- google.com (142.250.xxx.xx)
- github.com (20.207.xx.xx)
- youtube.com (142.250.xx.xx)
- Facebook services

================================================================================

KEY OBSERVATIONS

Network Type: IPv6 dominant (92.3% of traffic)
Security: Good - majority encrypted (TLS/HTTPS)
DNS Performance: Fast resolution, all queries successful
Connection Quality: No packet loss detected
Modern Protocols: QUIC in use for Google services

================================================================================

TOOLS USED

- Wireshark 4.2.2
- tshark (command-line analysis)
- Ubuntu 24.04
- Network interface: wlan0

================================================================================

FILE STRUCTURE

Task-5_Wireshark-Packet-Analysis/
├── README.md (this file - task summary)
├── notes.txt (theory and concepts learned)
├── report.txt (detailed step-by-step analysis)
├── Capture.pcapng (actual packet capture)
