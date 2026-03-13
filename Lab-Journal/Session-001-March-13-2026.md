# Lab Session 001 - March 13, 2026

## Objectives
- Set up virtualized home lab environment
- Conduct vulnerability assessment using Nessus
- Begin STIG compliance assessment

## Environment Built
- Installed VirtualBox hypervisor
- Deployed Windows Server 2019 VM
- Deployed Ubuntu Linux Server VM

## Tools Used
- Tenable Nessus Essentials
- DISA STIG Viewer 3.7.0

## Nessus Findings
| Severity | Finding | Status |
|----------|---------|--------|
| Medium | SMB Signing Not Required | Remediated |
| Low | ICMP Timestamp Disclosure | Open |

## STIG Findings
| V-Number | Title | Status |
|----------|-------|--------|
| V-205802 | Windows Installer Elevated Privileges | Remediated |
| V-205725 | Anonymous Access Named Pipes | Not a Finding |
| V-205724 | Anonymous Enumeration of Shares | Remediated |
| V-205663 | NTFS Volume Format | Not a Finding |
| V-205654 | Registry Value Confirmed | Not a Finding |
| V-205653 | Reversible Password Encryption | Not a Finding |
| V-205919 | LAN Manager Authentication | Remediated |
| V-205914 | Anonymous SAM Enumeration | Not a Finding |
| V-205913 | Anonymous SID/Name Translation | Not a Finding |

## Lessons Learned
- STIG language can be tricky, must read carefully
- Not all controls apply to standalone systems
- Nessus and STIG checking complement each other
- Documentation is just as important as technical work

## Next Steps
- Complete remaining Cat I STIG controls
- Run SCAP compliance checker
- Set up Splunk SIEM
