# Final Network Audit Report

| Port | Service | Version | Risk | Attack Vector |
|---|---|---|---|---|
| 21 | FTP | vsftpd 2.3.4 | CRITICAL | Backdoor exploit, Cleartext creds |
| 22 | SSH | OpenSSH 4.7 | MEDIUM | Brute-force |
| 23 | Telnet | Linux telnetd | HIGH | Unencrypted, should disable |
| 80 | HTTP | Apache 2.2.8 | HIGH | DVWA - SQLi, XSS |
| 445 | SMB | Samba 3.0.20 | CRITICAL | SMB exploit - usermap script |

Conclusion: Target is intentionally vulnerable. All ports are high risk. Recommended mitigation is to patch in production.

Proof Attached: Nmap .txt outputs + Wireshark screenshot
