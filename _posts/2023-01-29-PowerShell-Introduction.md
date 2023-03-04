---
menutitle:         "PowerShell Introduction"
description:       "Windows 10 comes with a powerful tool for system administration called PowerShell. PowerShell is a 
                    command-line tool that provides administrators with a way to automate tasks and manage the system more 
                    efficiently. In this blog post, we will discuss how to perform Windows 10 system administration with PowerShell."
category:          Tutorials
author:            "Steven Wilkins"
tags:              PowerShell Windows Tools Tutorial
---

{% include navigation.html %}

## Getting started with PowerShell 

Before you start using PowerShell, you need to make sure that it is installed on your Windows 10 computer. To do this, open the 
Start menu and search for "PowerShell". If PowerShell is installed, you should see it in the search results. If it's not installed, 
you can download it from Microsoft's website.

## Running PowerShell as an administrator 

To perform system administration tasks with PowerShell, you need to run PowerShell as an administrator. To do this, right-click the 
PowerShell icon in the Start menu and select "Run as administrator" from the context menu. You will be prompted to confirm that you 
want to run PowerShell as an administrator.

## Working with PowerShell cmdlets 

PowerShell provides a wide range of cmdlets (pronounced "command-lets") that you can use to manage Windows 10. Cmdlets are small 
programs that perform specific tasks, such as retrieving information about your system or configuring settings. To get a list of 
all available cmdlets, type "Get-Command" and press Enter.

### Here are some examples of PowerShell cmdlets that you can use for system administration: 

`Get-Process`: Retrieves information about running processes on your system. 
`Get-Service`: Retrieves information about running services on your system.
`Set-ExecutionPolicy`: Changes the PowerShell execution policy to allow or disallow scripts to run.
`Set-Service`: Starts, stops, or restarts a service.
`Get-EventLog`: Retrieves information from event logs.

## Using PowerShell scripts 

One of the most powerful features of PowerShell is the ability to create scripts that automate repetitive tasks. To create a 
PowerShell script, open Notepad or your preferred text editor and type your PowerShell commands. Save the file with a .ps1 extension, 
such as "myscript.ps1".

To run the script, open PowerShell as an administrator and type the path to the script file, including the .ps1 extension. For example, 
if your script is located in the Documents folder, you would type "C:\Users\username\Documents\myscript.ps1" and press Enter.

## Using PowerShell modules 

PowerShell modules are collections of cmdlets, scripts, and other files that can be imported into PowerShell to extend its functionality. 
Microsoft provides a number of modules for managing Windows 10, including the ActiveDirectory module for managing Active Directory, and 
the Hyper-V module for managing virtual machines.

To import a module into PowerShell, use the "Import-Module" cmdlet. For example, to import the ActiveDirectory module, type 
"Import-Module ActiveDirectory" and press Enter.

## Getting help with PowerShell 

Finally, if you need help with PowerShell, you can use the built-in help system. To get help on a specific cmdlet, type "Get-Help cmdletname" 
and press Enter. For example, to get help on the Get-Process cmdlet, you would type "Get-Help Get-Process".

In conclusion, PowerShell is a powerful tool for system administration in Windows 10. With its wide range of cmdlets, scripts, and modules, 
you can automate tasks and manage your system more efficiently. By following the tips outlined in this blog post, you can get started with 
PowerShell and take your Windows 10 system administration to the next level.
