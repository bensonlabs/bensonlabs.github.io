---
title: Re-Establish Domain Trust via PowerShell
parent: Fixes
tags: [Windows, PowerShell, Active Directory]
---

Problem  
The machine has lost its trust relationship with the domain controller, preventing domain logins.

Environment  
Windows 10/11 — LAPS local administrator access required.

Fix  
Log in with a local admin account and re-establish trust with PowerShell:
# $credential = Get-Credential
# Reset-ComputerMachinePassword -Server <DomainController> -Credential (Get-Credential)
