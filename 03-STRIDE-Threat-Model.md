# 03 - STRIDE Threat Register

| ID | Component | STRIDE | Threat Description | Mitigation | Priority |
|---|---|---|---|---|---|
| T01 | DVWA Login | Spoofing | Brute-force admin login | Lockout + MFA | P1 |
| T02 | Juice Basket API | Tampering | Change price via IDOR | Server-side validation | P1 |
| T03 | vsftpd 2.3.4 | Elevation | Backdoor to get root shell | Patch vsftpd | P1 |
| T04 | Feedback Form | Info Disclosure | SQL Injection dump users | Parameterized Query | P1 |
| T05 | File Upload | Denial of Service | Upload big shell to crash | File size check | P2 |
