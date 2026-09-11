# 02 - Asset Inventory & Data Flow

| Asset ID | Asset | IP | Data Type | Trust Level |
|---|---|---|---|---|
| A01 | Kali Linux | 192.168.56.10 | Tools & Credentials | Trusted |
| A02 | Metasploitable 2 | 192.168.56.11 | Fake PII, Vuln Services | Untrusted |
| A03 | Juice Shop | 192.168.56.12 | User DB, JWT, Payment | Untrusted |
| ID01 | Lab User (admin:password) | - | Login Credentials | Low |

## Trust Boundaries
T1: Kali (Trusted) -> [Host-Only Boundary] -> Victim VMs (Untrusted)
T2: User (Untrusted) -> Web App -> Database (Sensitive)

## Data Flow (DFD Level 0)
User Browser -> (HTTP Request) -> Web App (Juice Shop / DVWA) -> (SQL Query) -> MySQL Database
