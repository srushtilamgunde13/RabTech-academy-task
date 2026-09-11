## 1. TCP SYN Scan (Stealth)
Command: sudo nmap -sS 192.168.56.11 -oN syn-scan.txt

Output:
PORT     STATE SERVICE
21/tcp   open  ftp
22/tcp   open  ssh
23/tcp   open  telnet
25/tcp   open  smtp
80/tcp   open  http
139/tcp  open  netbios-ssn
445/tcp  open  microsoft-ds
3306/tcp open  mysql

## 2. Service Versioning
Command: sudo nmap -sV 192.168.56.11

Output:
21/tcp - vsftpd 2.3.4 (VULNERABLE - backdoor)
22/tcp - OpenSSH 4.7p1
80/tcp - Apache 2.2.8 (Ubuntu) - DVWA
445/tcp - Samba 3.0.20

## 3. OS Detection
Command: sudo nmap -O 192.168.56.11

Output:
OS: Linux 2.6.9 - 2.6.33 - Metasploitable

## 4. UDP Scan
Command: sudo nmap -sU 192.168.56.11

Output:
53/udp open domain
68/udp open dhclient
