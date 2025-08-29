# Explicit Credential Use Detection

**Case ID:** CRED-2025-017  
**Events:** 43  
**Event ID:** 4648  
**Severity:** HIGH

## Alert Summary
43 instances of explicit credential use detected - possible lateral movement.

## Technical Context
Event 4648 occurs when credentials are explicitly provided (RunAs, network logon with different credentials).

## Security Implications
- Potential privilege escalation
- Lateral movement attempts
- Credential theft and reuse

## MITRE ATT&CK
- T1078: Valid Accounts
- T1021: Remote Services
