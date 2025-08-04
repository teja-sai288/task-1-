# task-1-
network port scanning

📌 Objective
Perform a network scan on your local network to identify active devices and their open ports using Nmap. The goal is to understand network exposure and potential security risks.

🧰 Tools Used
Nmap – for scanning the local network and detecting open ports.
Wireshark (optional) – for analyzing network traffic during the scan.
📡 Steps Performed
Installed Nmap from the official website: https://nmap.org/download.html
Identified local IP range using:
ipconfig (Windows) / ifconfig (Linux/macOS)
Ran TCP SYN scan using:
nmap -sS 192.168.1.0/24

🧾 Sample Output
Nmap scan report for 192.168.1.10 Host is up (0.0010s latency). PORT STATE SERVICE 22/tcp open ssh 80/tcp open http

Nmap scan report for 192.168.1.15 Host is up (0.0012s latency). PORT STATE SERVICE 445/tcp open microsoft-ds

🚨 Risk Analysis
Port Service Risk 22 SSH Could be brute-forced if weak credentials 80 HTTP If outdated web server, can be exploited 445 SMB Commonly exploited by malware like WannaCry
