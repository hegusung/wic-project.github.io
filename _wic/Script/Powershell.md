---
Name: Powershell
Description: Powershell is a common scripting language on Windows environements
Author: 'Hegusung'
Created: 2024-10-23
Categories:
  - Category: COM Objects
    Description: Powershell - COM
    Usecase: Powershell can access and execute COM objects
    MitreID: T1546
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
  - Category: Windows API
    Description: Powershell - Windows API
    Usecase: Powershell can execute Windows API
    MitreID: T1106
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
  - Category: .Net Class
    Description: Powershell - .Net Class
    Usecase: Powershell can access functionalities from .Net classes
    MitreID: T1203
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
  - Category: WMI
    Description: VBScript - WMI
    Usecase: VBScript can execute a WMI Queries by leveraging com objects
    Code: |
      Get-WmiObject -Class Win32_OperatingSystem
    MitreID: T1546
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
  - Category: Download
    Description: Powershell - Download
    Usecase: Powershell can download a file from a remote server to a buffer or a file
    Code: |
      # Using Invoke-RestMethod to download to a buffer
      $buffer = Invoke-RestMethod -Uri "https://example.com/data.json"
      # Using Invoke-WebRequest to download to a file
      Invoke-WebRequest -Uri "https://example.com/file.zip" -Outfile "output.zip"
    MitreID: T1105
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
  - Category: Create Process
    Description: Powershell - Create Process
    Usecase: Powershell can start a process using Start-Process
    Code: |
      Start-Process "program.exe" -ArgumentList "arg1", "arg2", "arg3"
    MitreID: T1106
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
  - Category: Text File Manipulation
    Description: Powershell - Text File Manipulation
    Usecase: Powershell can create text files, useful to drop text-based payloads on the disk
    Code: |
      "Hello !" | Out-File -FilePath "C:\path\to\file.txt"
      Set-Content -Path "C:\path\to\file.txt" -Value "Hello !"
      Add-Content -Path "C:\path\to\file.txt" -Value "Hello !"
    MitreID: T1059
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
  - Category: Registry Manipulation
    Description: Powershell - Registry Manipulation
    Usecase: Powershell can create or modify registry keys using cmdlets
    Code: |
      New-Item -Path "HKCU:\Software\key"
      New-ItemProperty -Path "HKCU:\Software\key" -Name "Test" -Value "String Value" -PropertyType String
    MitreID: T1112
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
  - Category: Service Manipulation
    Description: Powershell - Service Manipulation
    Usecase: Powershell can create or modify services using cmdlets (requires Admin access)
    Code: |
      New-Service -Name "MyService" -DisplayName "My Service" -BinaryPathName "C:\path\to\bin.exe" -StartupType Automatic
    MitreID: T1031
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
  - Category: Scheduled Task Manipulation
    Description: Powershell - Scheduled Task Manipulation
    Usecase: Powershell can create or modify scheduled tasks using cmdlets
    Code: |
      # Define the Action
      $action = New-ScheduledTaskAction -Execute "C:\path\to\bin" -Argument "arg1 arg2 arg3"
      # Define the trigger
      $trigger = New-ScheduledTaskTrigger -Daily -At "09:00AM"
      # Register
      Register-ScheduledTask -Action $action -Trigger $trigger -TaskName "TaskName" -Description "Task Description" -User "SYSTEM" -RunLevel Highest
    MitreID: T1053
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
Detection:
Resources:
  - Link: https://hegusung.github.io/LOLBAS-Project-hegusung.github.io/#/powershell
Acknowledgement:
  - Person: Hegusung
    Handle: '@hegusung'
---
