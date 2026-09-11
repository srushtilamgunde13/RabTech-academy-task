## Wireshark Analysis

Capture File: wireshark-capture.pcapng (taken while logging into DVWA)
Filter Used: http || ftp || telnet

Findings:
1. Found HTTP login in cleartext:
   - POST /dvwa/login.php - username=admin & password=password - UNENCRYPTED - HIGH RISK

2. Found FTP credentials in cleartext:
   - FTP 21/tcp - USER msfadmin / PASS msfadmin - Visible in Wireshark

3. Anomalous Protocol:
   - Telnet 23/tcp is using unencrypted communication - should be disabled

Screenshot:
[Attach your Wireshark screenshot here - take screenshot of Wireshark showing http packet]
