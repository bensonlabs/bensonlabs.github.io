---
title: Re-Establish Domain Trust via PowerShell
parent: Fixes
tags: [Windows, PowerShell, Active Directory]
---

Problem  
The machine has lost its trust relationship with the domain controller, preventing domain logins.

Environment  
Windows 10/11 — local administrator access required.

Fix  
Log in with a local admin account and re-establish trust with PowerShell:

* skip this method
# Reset secure channel with domain
Test-ComputerSecureChannel -Repair -Credential (Get-Credential)

* Do this one first 
# Alternative (simpler but less interactive)
# Reset-ComputerMachinePassword -Server <DomainController> -Credential (Get-Credential)