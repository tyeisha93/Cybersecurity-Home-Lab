# POA&M Update Entry
## Plan of Action and Milestones — Cybersecurity Home Lab

| Field | Details |
|-------|---------|
| **POA&M ID** | POAM-001 |
| **Finding** | ICMP Timestamp Request Remote Date Disclosure |
| **CVE** | CVE-1999-0524 |
| **Severity** | Low |
| **Date Discovered** | March 2026 |
| **Status** | CLOSED |
| **Root Cause** | Windows Firewall profiles (Domain, Private, Public) were disabled on the VM preventing firewall rules from taking effect |
| **Remediation Steps** | 1. Enabled all three Windows Firewall profiles via PowerShell using Set-NetFirewallProfile command. 2. Created and enabled four Windows Firewall rules blocking ICMPv4 Type 13 inbound and Type 14 outbound. 3. Verified rules were active using Get-NetFirewallRule command. |
| **Verification Method** | Follow up Nessus Essentials scan conducted — zero Critical, High, Medium or Low findings remaining |
| **Date Closed** | March 28, 2026 |
| **Closed By** | Tyeisha Roberts |

## Evidence
![Final Clean Scan](../Nessus-Scans/Final%20scan.png)
