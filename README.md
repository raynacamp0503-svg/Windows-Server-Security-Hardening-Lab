# Windows-Server-Security-Hardening-Lab

## Overview
In this project, I hardened a Windows Server environment to reduce attack surface and improve monitoring. The goal was to apply practical security controls that are commonly used in enterprise environments.

## What I did
- Created accounts and applied least privilege permissions
- Enforced password and account policies using Group Policy
- Enabled auditing for successful and failed security events
- Hardened endpoint protections (Windows Defender / security settings)
- Disabled legacy/insecure protocols (ex: SMBv1, NTLM, PowerShell 2.0)
- Configured logging and monitoring (ex: DNS logging, PowerShell logging)
- Supported patching / update configuration to reduce known vulnerabilities

## Tools & Technologies
- Windows Server
- Active Directory / Local Security Policy
- Group Policy Editor (GPO)
- PowerShell
- Windows Defender & Firewall
- Windows Event Logging / DNS logging

## Evidence
Screenshots are included in the `screenshots/` folder and the full lab report is in `report/`.

## Key Takeaway
This lab helped me practice securing and monitoring a Windows Server environment using real-world hardening steps and security controls.
