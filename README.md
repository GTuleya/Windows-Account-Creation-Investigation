# Windows Account Creation Investigation – Event ID 4720

## Objective
Investigate Windows Security Event ID 4720 to identify newly created user accounts and determine whether the activity is authorized or potentially suspicious.

## Tools Used
- Windows Event Viewer
- Windows Command Prompt
- Windows Security Auditing

## Investigation Steps
1. Opened Command Prompt as administrator.
2. Enabled User Account Management auditing using AuditPol.
3. Created a temporary local Windows account named SOCLabTest.
4. Opened Windows Event Viewer.
5. Navigated to Windows Logs > Security.
6. Filtered security events for Event ID 4720.
7. Examined the account creation details.
8. Verified that security auditing was enabled.
9. Removed the temporary test account after completing the investigation.

## Findings
- **Event ID:** 4720
- **Event Description:** A user account was created.
- **Account Created:** SOCLabTest
- **Date:** November 13, 2026
- **Time:** 12:57:40 PM
- **Result:** Audit Success
- **Assessment:** Authorized account creation performed for cybersecurity training.

## Security Significance
Unexpected user account creation could indicate unauthorized access or an attempt to maintain access to a system. A SOC Analyst should identify who created the account, verify whether the activity was approved, and investigate other related security events.

## Conclusion
This lab demonstrated how to enable Windows account management auditing, investigate Windows Security Event ID 4720, identify newly created user accounts, and document findings.

## Evidence
- Event ID 4720 screenshot
- Windows audit policy screenshot
