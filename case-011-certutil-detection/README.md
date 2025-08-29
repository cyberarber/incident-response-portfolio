# Living-off-the-Land Binary Detection: Certutil.exe

**Case ID:** LOLBIN-2025-011  
**Date:** August 28, 2025  
**Severity:** HIGH  

## Detection
Successfully identified certutil.exe execution via Event 4688 with full command line logging.

## Event Details
- Process: C:\Windows\System32\certutil.exe
- Detection Time: 23:02:27.404
- Host: DESKTOP-5I4MQEU
- User: win10

## Threat Context
Certutil.exe is commonly abused by attackers for:
- Downloading malicious files
- Base64 encoding/decoding payloads
- Certificate manipulation

## MITRE ATT&CK
- T1105: Ingress Tool Transfer
- T1140: Deobfuscate/Decode Files
- T1218: System Binary Proxy Execution

