---
Name: DDE
Description: Dynamic Data Exchange (DDE) is an inter-process communication method used in Windows to allow applications to share data and commands in real-time, enabling features such as embedding objects and automating tasks between software like Microsoft Excel and other applications.
Author: 'Hegusung'
Created: 2024-10-25
Categories:
  - Category: CMD
    Description: DDE - Command execution
    Usecase: Execute a command through a Excel file
    MitreID: T1204
    OperatingSystem: Windows XP, Windows 7, Windows 8, Windows 10, Windows 11
    Code: |
      =CMD|' /C calc.exe'!A0
    Code_Sample:
    Tags:
      - Origin: Clickable
Detection:
Resources:
Acknowledgement:
---
