---
layout: post
title: "Setting up the Windows PowerShell profile in Windows"
date: 2012-08-20 18:51
comments: true
categories: ["Windows", "Visual Studio", "Setup"]
---

Here's how to make the Windows PowerShell command-line prompt use the Visual Studio 2012 environment variables and settings:

1.  We have to start by allowing the loading of PowerShell configuration and profile files, which is disabled by default. To that end, execute the following in a PowerShell window started with admin rights (confirm you want to change the execution policy when prompted):

        PS> Set-ExecutionPolicy Unrestricted

2.  Copy the PowerShell profile file from **devsetup/Windows/Microsoft.PowerShell_profile.ps1** into **My Documents/WindowsPowerShell**, ensuring the filename is preserved exactly.

3.  That's it. You can now use the Visual Studio command-line tools from PowerShell.