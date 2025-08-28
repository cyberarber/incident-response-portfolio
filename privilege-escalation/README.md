# Privilege Escalation Investigation

**Date:** August 27, 2025  
**Platform:** Elastic Stack  
**Analyst:** Arber Kycyku  

## Detection Query
event.code: "4672" OR event.code: "4624"

## Key Findings
- 2,624 security events detected
- Event 4672: Special privileges assigned to new logon
- Event 4624: Successful logon
- Host: DESKTOP-C4AJTEF (Windows 11 Enterprise)

## Investigation Notes
Special privilege events (4672) indicate admin rights were granted. This is normal for legitimate admin users but suspicious when:
- Occurring outside business hours
- Associated with service accounts
- Following failed login attempts

## Response Actions
1. Verified user identity
2. Checked authorization for elevated access
3. Reviewed audit logs for suspicious commands
4. No malicious activity confirmed

