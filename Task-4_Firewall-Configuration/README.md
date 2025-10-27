# Task 4: Firewall Configuration with UFW

Name: Krushal Hirpara
Date: 25 October 2025

================================================================================

SUBMISSION FILES

1. README.md - This file (overview and quick steps)
2. report.txt - Step-by-step practical with observations
3. notes.txt - Short theory (firewall basics and UFW)
4. image.png - UFW log screenshot (masked for privacy)

================================================================================

TASK SUMMARY

- Set secure defaults: deny incoming, allow outgoing
- Allowed SSH (22/tcp) before enabling UFW to avoid lockout
- Denied Telnet (23/tcp) and verified with telnet/nc (connection refused)
- Temporarily allowed HTTP/HTTPS (80/443) to see rule behavior
- Spun up example services (HTTP on 8080, FTP on 21, nc on 9999) and scanned with nmap
- Practiced IP allow/deny rules, numbered rule deletion, logging, reset/disable/enable

================================================================================

QUICK START (COMMANDS)

1) Defaults and enable
	- which ufw → /usr/sbin/ufw
	- sudo ufw default deny incoming
	- sudo ufw default allow outgoing
	- sudo ufw allow 22/tcp
	- sudo ufw enable

2) Block Telnet (verify)
	- sudo ufw deny 23/tcp
	- telnet localhost 23 → Connection refused

3) Check rules
	- sudo ufw status numbered

Optional (demo services and scan)
	- python3 -m http.server 8080 &
	- sudo systemctl start vsftpd
	- sudo netstat -tuln | grep LISTEN
	- nmap -F localhost

================================================================================

NOTES

- Loopback (127.0.0.1) scans show local daemons even with “deny incoming”; UFW’s inbound policy targets external ingress.
- Always add the SSH rule before enabling UFW on remote hosts.
- Use numbered status to safely delete specific rules.
