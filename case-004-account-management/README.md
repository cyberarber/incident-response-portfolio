# Account Management Audit

**Case ID:** ACC-2025-004  
**Date:** August 28, 2025  
**Analyst:** Arber Kycyku  
**Severity:** Medium

## Executive Summary
Detected 8 account management events including audit policy changes on DESKTOP-C4AJTEF between July 31 and August 28, 2025.

## Events Detected
- Event 4722: User account enabled (1 event)
- Event 4738: User account changed (3 events)  
- Event 4720: User account created (2 events)
- Event 4724: Password reset attempt (2 events)

## Key Findings
- Host: DESKTOP-C4AJTEF (Windows 11 Enterprise)
- Time: 03:52:19 on Aug 28, 2025
- Provider: Microsoft-Windows-Security-Auditing
- All events occurred within same minute (suspicious clustering)

## Investigation Notes
Rapid succession of account modifications within 1 minute suggests:
1. Administrative maintenance window
2. Potential privilege escalation attempt
3. Account takeover scenario

## MITRE ATT&CK Mapping
- T1098: Account Manipulation
- T1078: Valid Accounts

## Response Actions
1. Verified account changes were authorized
2. Reviewed audit logs for context
3. No malicious activity confirmed

