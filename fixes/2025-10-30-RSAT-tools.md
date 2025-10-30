---
title: Install RSAT Tools via PowerShell
parent: Fixes
tags: [Windows, PowerShell, Active Directory]
---

# This installs AD Users and Computers and Group Policy Management
Add-WindowsCapability -Online -Name RSAT:ActiveDirectory-DomainServices; Add-WindowsCapability -Online -Name RSAT:GroupPolicy-Management
