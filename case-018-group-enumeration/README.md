# Security Group Enumeration Detection

**Case ID:** ENUM-2025-018  
**Events:** 614 total  
- Event 4798: 160 (Group membership enumerated)
- Event 4799: 454 (Security-enabled group enumerated)

## Detection Analysis
Significant group enumeration activity suggesting:
- Active Directory reconnaissance
- Privilege escalation preparation
- Insider threat activity

## Attack Pattern
Attackers enumerate groups to:
1. Identify high-privilege groups
2. Find lateral movement paths
3. Map organization structure

## MITRE ATT&CK
- T1069: Permission Groups Discovery
- T1087: Account Discovery
