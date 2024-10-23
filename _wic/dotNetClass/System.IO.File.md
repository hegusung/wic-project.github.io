---
Name: System.IO.File
Description: System.IO.File is a .Net Class which can be used to modify the filesystem
Author: 'Hegusung'
Created: 2024-10-23
Categories:
  - Category: File Manipulation
    Description: System.IO.File - File Manipulation
    Usecase: System.IO.File can create files, useful to drop payloads on the disk
    Code: |
      # Using WriteAllBytes
      [System.IO.File]::WriteAllBytes("C:\path\to\file.bin", $binaryData)
      # Using FileStream
      $filestream = [System.IO.File]::OpenWrite("C:\path\to\file.bin")
      $filestream.Write($binaryData, 0, $binaryData.Length)
      $filestream.Close()
    MitreID: T1059
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
