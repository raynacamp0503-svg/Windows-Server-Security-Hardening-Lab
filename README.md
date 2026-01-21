# Windows Server Security Hardening Lab

## Overview
This project demonstrates how I secured a Windows Server environment by applying enterprise-level hardening controls, reducing attack surface, and enabling monitoring for suspicious activity. The goal was to configure the system the same way it would be secured in a real production environment.

---

## Environment
- Windows Server 2022
- Local Security Policy & Group Policy Editor
- Active Directory (local users)
- PowerShell
- Windows Defender & Firewall
- DNS Manager

---

## Security Hardening Evidence

### 1. Password & Account Security
- Enforced strong password complexity, minimum length, and expiration policies
- Disabled the built-in Guest account to remove a common attack vector
- Implemented account lockout policies to prevent brute-force attacks

---

### 2. Logging, Auditing & Monitoring
- Enabled audit logging for account management, logon/logoff, privilege use, and system events
- Configured PowerShell script block logging to detect malicious script execution
- Enabled DNS debug logging to monitor suspicious domain queries

---

### 3. Least Privilege & Access Control
- Created restricted folders with explicit deny rules for non-admin users
- Configured UAC to always notify on system changes
- Restricted access to Control Panel, Command Prompt, and software installation

---

### 4. Credential & Authentication Hardening
- Disabled NTLM authentication to prevent relay and credential theft attacks
- Forced NTLMv2 for stronger authentication
- Prevented storage of LAN Manager hashes
- Enabled Credential Guard and Windows Defender protections

---

### 5. Network & Protocol Hardening
- Enabled Windows Firewall for all network profiles
- Disabled SMB 1.0, PowerShell 2.0, FTP, Telnet, Proxy services, SSDP, and UPnP
- Enabled SMB encryption to protect data in transit

---

### 6. Patch Management & Endpoint Protection
- Enabled automatic Windows Updates for continuous patching
- Enabled real-time and cloud-delivered antivirus protection
- Reduced exposure to known vulnerabilities

---

## Key Takeaways
This lab helped me practice securing a Windows Server system using real-world hardening techniques commonly used by security teams and system administrators. It strengthened my understanding of identity security, monitoring, attack surface reduction, and defensive security controls.

---

## Note on Redaction
All screenshots have been redacted to remove names, usernames, hostnames, SIDs, and identifiers in accordance with security best practices.
