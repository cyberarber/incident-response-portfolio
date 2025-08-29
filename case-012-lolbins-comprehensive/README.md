# Living-off-the-Land Binaries Detection Suite

**Case ID:** LOLBIN-2025-012  
**Date:** August 28, 2025  
**Analyst:** Arber Kycyku  
**Severity:** CRITICAL  

## Executive Summary
Successfully detected 8 instances of Living-off-the-Land Binary abuse across 4 different Windows system binaries.

## Detection Statistics
| Binary | Detections | Risk Level |
|--------|------------|------------|
| rundll32.exe | 4 | Critical |
| PowerShell.exe | 2 | Critical |
| bitsadmin.exe | 1 | High |
| certutil.exe | 1 | High |
| **Total** | **8** | **Critical** |

## Detailed Findings

### Rundll32.exe (4 detections)
- Execution path: C:\Windows\System32\rundll32.exe
- Used for DLL execution bypass
- Can execute JavaScript/VBScript

### PowerShell.exe (2 detections)
- Path: C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe
- Detected encoded command execution
- Primary tool for fileless malware

### Bitsadmin.exe (1 detection)
- Background Intelligent Transfer Service
- Used for downloading malicious payloads
- Legitimate Windows binary abuse

### Certutil.exe (1 detection)
- Certificate utility abused for file downloads
- Base64 encoding/decoding capabilities

## MITRE ATT&CK Coverage
- T1218: Signed Binary Proxy Execution
- T1059.001: PowerShell
- T1105: Ingress Tool Transfer
- T1140: Deobfuscate/Decode Files
- T1055: Process Injection

## Detection Capabilities Validated
Event 4688 with command line auditing successfully captures all LOLBin executions, providing critical visibility into potential abuse of legitimate Windows binaries.

