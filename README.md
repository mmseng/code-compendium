# Matt's code compendium

## About

### Me
My name is Matt Seng. I've been an IT Pro for higher education since 2007. This is a list of projects I've done, mostly Powershell-based.  

My Github.com username is mmseng, but the majority of my scripting work is done for the purposes of system administration for the Grainger College of Engineering at the University of Illinois, where my NetID is mseng3.  

If you wish to contact me about my work, please use the University's Microsoft Teams system to do so. If you can't, then email to my university email will suffice. For now, I will not monitor communications here on GitHub.  

### Access
Currently much of my work is stored on version control systems internal to the college, though eventually it will be slowly migrated to the university's GitHub.com organizations, which is why I've spun up this page/repo, and I'll try to keep it updated with the current locations of my projects.  

If you do not have access to a project linked below and are interested in getting access, please contact me per the above.  

## Compendium
The following is a list of the major scripts/modules/projects I've made, roughly organized by their current location and purpose.

### EPM/MECM focus (GitLab group engrit-epm)

#### "Org shared deployment model"
Standardization of MECM collections and deployments across the college.  
https://gitlab.engr.illinois.edu/engrit-epm/org-shared-deployments

#### Compare-AssignmentRevisions
Collects MECM client data directly from mass endpoints for analysis to identify issues related to deployment bugs in MECM 
https://gitlab.engr.illinois.edu/engrit-epm/compare-assignmentrevisions

#### Get-AppSupersedence
Analyzes data from MECM to identify mis-configured application packages, which cause deployment issues 
https://gitlab.engr.illinois.edu/engrit-epm/get-appsupersedence

#### Eval-SccmDeviceAssignments
Forcing MECM client endpoints to re-evaluate assignments
Credit goes to UIUC Endpoint Services (EPS) team
https://gitlab.engr.illinois.edu/engrit-epm/eval-sccmdeviceassignments

#### Export-PrintServerPrinters
A script to grab printer data from our print servers, and dump it to a CSV format, suitable for consumption by my PrinterStatus webtool (mentioned below).
https://gitlab.engr.illinois.edu/engrit-epm/export-printserverprinters

---

### System administration/AD focus (GitLab group: oesr, a.k.a. Official EngrIT Script Repo)

#### 
Auditing of "stale" AD computer accounts, and bulk remediation
https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Audit-StaleADComputersInOU

---

### System administration (hosted on personal GitHub)

#### bcdedit-revert-uefi-gpt-boot-order
Automating the correction of Windows UEFI boot order after installation of Windows modifies it
https://github.com/mmseng/bcdedit-revert-uefi-gpt-boot-order

---

### Generalized topics which I have experience with, but don't represent specific code projects
- Misc gathering, reporting, and manipulation of MECM data 

---





Directly polling endpoints to identify where certain applications are installed 

Resetting of administrator account passwords as securely as possible without leveraging something like LAPS 

Automation of refactoring AD OUs and GPOs to facilitate segregated remote access for COVID remote work purposes 

Automation of provisioning and decommissioning mass guest AD accounts, and role-based accounts and groups (for events, classes, research groups, etc.) 

Auditing readiness of Win7 systems to accept Extended Service Updates (ESUs) 

Identifying and sending commands to AD endpoints based on status of local and/or remote session activity 

Gathering data directly from endpoints such as diskspace, session activity, uptime, make/model, and other data provided by WMI/CIM and Remote Management (RM) frameworks. 

Web-based tool (leveraging Jenkins) for automation of importing new computer information to AD, MECM, and IPAM 

MECM task sequence steps for gathering endpoint's LENS data and sending notifications with said data to Slack and MS Teams 

Misc gathering, reporting, and manipulation of AD data 

Misc gathering, reporting, and manipulation of LENS data 

Quick functions for various handy administrative tasks, such as mass asynchronous pinging, recording ping responses over time, polling user's homedirectory for quota and other stats 

Customization of Powershell profile, with automatic import of various modules, such as those mentioned above 

Long list of misc syntax, cmdlets, and snippets I've found handy over the years 

General practice of thorough process logging for scripts for easy troubleshooting and review 

I've done lots of process improvement and technical documentation for various projects and workflows for the org, with a focus on efficiency, leveraging new technology, security, and ease of use and accessibility for student workers, staff with limited training, or minimal permissions. 

Not Powershell, but PHP: one-stop-shop web-based status monitoring (leveraging the SNMP protocol) for all of the college's printers 
