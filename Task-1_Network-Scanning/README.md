# Task 1: Network Port Scanning with Nmap

Name: Krushal Hirpara
Date: 20 October 2025

================================================================================

SUBMISSION FILES

1. README.md - This file
2. report.txt - Complete scan outputs
3. scan_results.txt - Raw nmap output
4. notes.txt - Quick notes

================================================================================

TASK SUMMARY

Scanned local network XXX.XXX.X.0/24 using Nmap 7.94SVN

Active Hosts Found: 2

Gateway (XXX.XXX.X.X):
- Port 53/TCP - DNS
- Port 53/UDP - DNS
- Port 67/UDP - DHCP

My Computer (XXX.XXX.X.XXX):
- Port 80/TCP - Apache httpd 2.4.58

Localhost Services:
- Port 631/TCP - IPP
- Port 3306/TCP - MySQL
- Port 5432/TCP - PostgreSQL

================================================================================

SCAN TYPES PERFORMED

- Basic host scan
- TCP SYN scan (-sS)
- Service version detection (-sV)
- Fast scan (-F)
- Aggressive scan (-A)
- UDP scan (-sU)
- Ping scan (-sn)

================================================================================

Note: IP addresses and MAC addresses masked for privacy (XXX format)

================================================================================