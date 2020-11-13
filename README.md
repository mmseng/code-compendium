# Matt's code compendium

## About

### Me
My name is Matt Seng. I've been an IT Pro for higher education since 2007. This is a list of projects I've done, mostly Powershell-based.  

My Github.com username is mmseng, but the majority of my scripting work is done for the purposes of system administration in my work for Engineering IT Shared Services, in the Grainger College of Engineering at the University of Illinois, where my NetID is mseng3.  

If you wish to contact me about my work, please use the University's Microsoft Teams system to do so. If you can't, then email to my university email will suffice. For now, I will not monitor communications here on GitHub.  

### Access
Currently much of my work is stored on version control systems internal to the college, though eventually it will be slowly migrated to the university's GitHub.com organizations, which is why I've spun up this page/repo, and I'll try to keep it updated with the current locations of my projects.  

If you do not already have access to a project linked below and are interested in getting access, please contact me per the above. Some projects are already public, some are not, so try the links first. For projects hosted on gitlab.engr-illinois.edu, you must sign in there at least once, so that your account will be generated and can be granted access.

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
Grabs printer data from our print servers, and dumps it to a CSV format, suitable for consumption by my PrinterStatus webtool (mentioned below).
https://gitlab.engr.illinois.edu/engrit-epm/export-printserverprinters

#### Report-ProductVersion
Directly polls endpoints to identify where certain applications are installed, and what the installed version is.
https://gitlab.engr.illinois.edu/engrit-epm/report-productversion

#### PWResetV2
Resetting of administrator account passwords as securely as possible without leveraging something like LAPS
Contact for more information.

#### Helptools Importer
Web-based tool (leveraging Jenkins) for automation of importing new computer information to AD, MECM, and IPAM
https://gitlab.engr.illinois.edu/engrit-epm/helptools-importer

#### 
MECM task sequence steps for gathering endpoint's LENS data and sending notifications with said data to Slack and MS Teams 
https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/get-lens-info.ps1
https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/post-to-slack.ps1
https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/post-to-teams.ps1

---

### System administration/AD focus (GitLab group: oesr, a.k.a. Official EngrIT Script Repo)

#### 
Auditing of "stale" AD computer accounts, and bulk remediation
https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Audit-StaleADComputersInOU

#### Covidize-LabOU
Automation of refactoring AD OUs and GPOs to facilitate segregated remote access for COVID remote work purposes 
https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Covidize-LabOU

#### "Bulk AD account and group provisioning"
Automation of provisioning and decommissioning mass guest AD accounts, and role-based accounts and groups (for events, classes, research groups, etc.) 
Recycle-EWSGuestAccounts: https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Recycle-EWSGuestAccounts
Creating role-based accounts and groups: https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/create-role-based-ad-accounts-and-groups
Bulk creation of semesterly class accounts: https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Create-ICTDocClassAccounts

#### Validate-Win7ESUCompat
Auditing readiness of Win7 systems to accept Extended Service Updates (ESUs) 
https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Validate-Win7ESUCompat

#### "Manipulating computers based on session state"
Identifying and sending commands to AD endpoints based on status of local and/or remote session activity 
https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-Sessions
https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-ComputersBySessionState
https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Logoff-DisconnectedSessions

#### "Misc direct data gathering via WMI/RM"
Gathering data directly from endpoints such as diskspace, session activity, uptime, make/model, and other data provided by WMI/CIM and Remote Management (RM) frameworks. 
https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-Model
https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-DiskSpace
https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-UptimeHistory

#### "Misc handy snippets"
Long list of misc syntax, cmdlets, and snippets I've found handy over the years
https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/misc-handy-powershell-examples

---

### System administration (hosted on personal GitHub)

#### bcdedit-revert-uefi-gpt-boot-order
Automating the correction of Windows UEFI boot order after installation of Windows modifies it
https://github.com/mmseng/bcdedit-revert-uefi-gpt-boot-order

---

### Non-powershell projects

#### PrinterStatus
One-stop-shop web-based status monitoring (leveraging the SNMP protocol) for all of the college's printers
https://helptools.engrit.illinois.edu/tools/printerstatus/

---

### Generalized topics which I have at least some experience with, but which don't represent specific code projects
- Misc gathering, reporting, and manipulation of MECM data
- Misc gathering, reporting, and manipulation of AD data
- Misc gathering, reporting, and manipulation of LENS data
- Misc gathering, reporting, and manipulation of IPAM data
- Quick functions for various handy administrative tasks, such as mass asynchronous pinging, recording ping responses over time, polling user's homedirectory for quota and other stats
- Customization of Powershell profile, with automatic import of various modules, such as those mentioned above 
- General practice of thorough process logging for scripts for easy troubleshooting and review 

## Notes
- By mseng3
