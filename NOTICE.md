## Purpose

* The WIC Project is a community-driven open-source resource for documenting Windows components which can be used by threat groups to infect Windows systems.

* Please refer to the README.md for "Windows-Infection-Components" criteria and definition.

* "WIC Project" and "WIC" are used interchangeably in this document and refer to the "WIC Project"

## Project License

* The WIC Project is licensed under GPL 3.0. For license information, please refer to the [LICENSE file](/LICENSE).

## Definitions

* Submitter: An individual, group, organization, or entity that contributes to the WIC project through project maintenance, issue submission, Pull Request (PR) submission, etc.
* Consumer: An individual, group, organization, or entity that uses ("consumes") the WIC project resources through the web portal or repository interfaces and capabilities.

## Project Terms of Use & Disclaimers

* The content presented in the WIC Project, an open-source project, is for educational and informational purposes only. By using this project, including information presented on all project pages and resources in the project repository, you agree that the project authors and maintainers shall not be liable and/or held responsible/accountable for any damages resulting from the presentation, use, or misuse of the information contained on any project pages and repository documents.

* The WIC Project does NOT claim that detection resources/information provided on any project pages and repository documents offer complete and proper defensive/analytic coverage for documented and undocumented WIC commands, techniques, and/or use cases. 

* The WIC project is a consumable resource for commercial entities, private entities, and individuals. WIC includes and references resources from open and public sources to enhance content quality, however, the WIC Project does not endorse any particular entity, vendor, project, group, or individual. Furthermore, use of the WIC project or any WIC site/repository content by commercial entities, private entities, and individuals does not imply endorsement.

* WIC references and links to many external/3rd party resources. Linked sites and references are not under the control of the WIC Project, and as such, the WIC Project is not responsible for content of external/3rd party resource sites. Furthermore, linking of external/3rd party resources does not imply endorsement of those who manage or maintain those resources.

## Project Usage

* For consuming content on the WIC Project, please refer to the content on this page, navigate to resources under [/yml](/yml), and/or visit: https://wic-project.github.io.
* For making a contribution to the WIC Project, please refer to this notice, [README.md](/README.md), and [CONTRIBUTING.md](/CONTRIBUTING.md).

## WIC Entry Structure & Information

* `Name` Field: The name of the WIC file type or component resource.

* `Description` Field: A short sentence of the legitimate functionality of the 'wic' resource.

* `Author` Field: The submitter of the 'wic' resource.

* `Created` Field: The date when the 'wic' resource is submitted or this entry is created.

* TODO

* `Components` Field: Contains subfields to describe usage of the 'wic' resource. Includes:
  * `Description` (details of the 'lol' command behavior);
  * `Usecase` (details of the use case such as the purpose and technique;
  * `Category` (Category of the WIC);
  * `Privilege` (User or Administrator level privileges required);
  * `MitreId`[^1] (MITRE (R) ATT&CK(R) Tactic/Technique mapping);
  * `OperatingSystem` (version such as Windows 10).

* `Code Sample` Field: Includes the `Code` subfield to specify a link to a code snippet (if applicable).

* `Detection` Field: Contains subfields to describe potential detection criteria of the 'lol' resource. Includes:
  * `Sigma`[^2] (a link to Sigma detection rule on Sigma's git repository);
  * `Splunk`[^2] (a link to Splunk detection rule on Splunk's git repository);
  * `Elastic`[^2] (a link to Elastic detection rule on Elastic's git repository);
  * `IOC`[^3] (to provide information about indicators of compromise);
  * `Analysis`[^4] (a placeholder for linked resources - e.g. blog, gist, write-up, Twitter post, etc.).

* `Resources` Field[^5]: The `Link` subfield is a placeholder for a referenced resource link about the 'lol' resource.

* `Acknowledgements` Field: Includes the following subfields:
  * `Person` (identifies the individual who originally discovered the technique/command);
  * `Handle` (the person's Twitter handle if applicable).


[^1]: Note on MITRE(R) ATT&CK(R) Reference Model: Since the ATT&CK(R) model is widely adopted, WIC attempts map to the appropriate technique if applicable. The applicable ATT&CK(R) license appears in the 'Licenses' section.

[^2]: Note on Detection References: WIC does not guarantee that a particular detection reference included by a submitter/maintainer will detect associated WIC behavior. The reference is simply an acknowledgment that a resource exists, and the resource could potentially be useful for a consumer. Furthermore, WIC does not endorse any referenced project over another, but rather, appreciates the efforts made by individuals and organizations for providing publicly available resources/projects. Consumers of such projects are encouraged to understand a referenced project's Terms of Use and abide by the project's licensing criteria if applicable. 

[^3]: Note on Detection IOCs: WIC does not guarantee that a particular detection IOC included by a submitter/maintainer will detect associated WIC behavior.

[^4]: Note on Detection Analysis Links: A linked analysis resource under the Detection Field (e.g. blog, gist, write-up, etc.) and contents provided by a submitter/maintainer are not endorsed by the WIC project. However, WIC does appreciate the efforts made by individuals and organizations for providing publicly available resources. Consumers of the 'Analysis' resource are encouraged to understand the respective resource's Terms of Use and abide by the resource's licensing criteria if applicable.

[^5]: Note on Resource Links: A linked resource under the Resources Field (e.g. blog, gist, write-up, Twitter post, etc.) and contents provided by submitters/maintainers are not endorsed by the WIC project. However, WIC does appreciate the efforts made by individuals and organizations for providing publicly available resources. Consumers of the linked resource are encouraged to understand the respective resource's Terms of Use and abide by the resource's licensing criteria if applicable.

## MITRE ATT&CK License

* MITRE ATT&CK Terms of Use Link: https://attack.mitre.org/resources/terms-of-use/

LICENSE
The MITRE Corporation (MITRE) hereby grants you a non-exclusive, royalty-free license to use ATT&CK® for research, development, and commercial purposes. Any copy you make for such purposes is authorized provided that you reproduce MITRE's copyright designation and this license in any such copy.

"© 2021 The MITRE Corporation. This work is reproduced and distributed with the permission of The MITRE Corporation."

DISCLAIMERS
MITRE does not claim ATT&CK enumerates all possibilities for the types of actions and behaviors documented as part of its adversary model and framework of techniques. Using the information contained within ATT&CK to address or cover full categories of techniques will not guarantee full defensive coverage as there may be undisclosed techniques or variations on existing techniques not documented by ATT&CK.

ALL DOCUMENTS AND THE INFORMATION CONTAINED THEREIN ARE PROVIDED ON AN "AS IS" BASIS AND THE CONTRIBUTOR, THE ORGANIZATION HE/SHE REPRESENTS OR IS SPONSORED BY (IF ANY), THE MITRE CORPORATION, ITS BOARD OF TRUSTEES, OFFICERS, AGENTS, AND EMPLOYEES, DISCLAIM ALL WARRANTIES, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTY THAT THE USE OF THE INFORMATION THEREIN WILL NOT INFRINGE ANY RIGHTS OR ANY IMPLIED WARRANTIES OF MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE.

## Other Notices

* Microsoft(R) Windows(R) is a registered trademark of the Microsoft Corporation
