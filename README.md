# Matt's code compendium

## Me
I've been an IT pro for higher education since 2007. This is a list of some projects I've done, mostly Powershell-based, which I felt are worth sharing for other IT pros.  

My Github.com username is mmseng, but the majority of my scripting work is done for the purposes of system administration for Engineering IT Shared Services, in the Grainger College of Engineering at the University of Illinois, where my NetID is mseng3.  

If you wish to contact me about my work, please use the University's Microsoft Teams system to do so, either directly or through the PowerShell User Group team. If you can't, then my university email will suffice. For now, I will not monitor communications here on GitHub.  

## Access
Currently much of my work is stored on version control systems internal to the college, though I am working on migrating it to the university's GitHub.com organizations and made public (where possible), which is why I've spun up this page/repo, and I'll try to keep it updated with the current locations of my projects.  

In the table below, a visibility of `Private` means the code is hosted on Engineering IT's "internal" GitLab service and is only accessible to those specifically granted access. `Public` means the code is accessible to the whole internet. `University` means the code is accessible to any member of any organization belonging to University of Illinois' enterprise-wide GitHub license (i.e. basically any university affiliate).  

If you are interested in getting access to a project which is still private, please contact me per the above. For projects hosted on gitlab.engr-illinois.edu, you must sign in there at least once, so that your account will be generated and can be granted access.  

## Compendium

 | Name and link | Description | Type | Language | Visibility | 
 | ------------- | ----------- | ---- | -------- | ---------- | 
 | [Recycle-EWSGuestAccounts](https://github.com/engrit-illinois/Recycle-EWSGuestAccounts) | Bulk provisioning and decommissioning of guest AD accounts | bulk manipulation, scripting of repetitive processes | Powershell | University | 
 | [create-role-based-ad-accounts-and-groups](https://github.com/engrit-illinois/create-role-based-ad-accounts-and-groups) | Creation of role-based AD accounts and groups, i.e. for administrative use, research groups, and RSOs | bulk manipulation, scripting of repetitive processes | Powershell | University | 
 | [Create-ICTDocClassAccounts](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Create-ICTDocClassAccounts) | Bulk creation of guest AD accounts, i.e. for a semesterly community class | Bulk manipulation, scripting of repetitive processes | Powershell | Private | 
 | [get-lens-info](https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/get-lens-info.ps1) | Gathers data about the local endpoint's MAC from LENS data and saves it in MECM task sequence variables | info gathering/reporting | Powershell | Public | 
 | [post-to-slack](https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/post-to-slack.ps1) | Sends a message to a Slack channel | info gathering/reporting | Powershell | Public | 
 | [post-to-teams](https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/post-to-teams.ps1) | Sends a message to a MS Teams channel | info gathering/reporting | Powershell | Public | 
 | [Get-Sessions](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-Sessions) | Gets session data from remote endpoints, and returns it in a proper Powershell object | info gathering/reporting | Powershell | Public | 
 | [Get-ComputersBySessionState](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-ComputersBySessionState) | Gets a list of computers which have sessions matching given criteria | info gathering/reporting | Powershell | Public | 
 | [Get-Model](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-Model) | Gets model and other info (WMI Win32_ComputerSystem class) from remote endpoints | info gathering/reporting | Powershell | Private | 
 | [Get-DiskSpace](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-DiskSpace) | Gets available and free disk space from remote endpoints, caluclates free space %, and highlights endpoints with low free space | info gathering/reporting | Powershell | Private | 
 | [Get-UptimeHistory](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-UptimeHistory) | Retrieves precise uptime history from a remote endpoint | info gathering/reporting | Powershell | Private | 
 | [Get-FormFactors](https://github.com/engrit-illinois/Get-FormFactors) | Gets form factor and other info (WMI Win32_SystemEnclosure and Win32_ComputerSystem classes) from remote endpoints | info gathering/reporting | Powershell | Public | 
 | [misc-handy-powershell-examples](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/misc-handy-powershell-examples) | Long list of misc syntax, cmdlets, and snippets I've found handy over the years | misc | Powershell | Private | 
 | [org-shared-deployments](https://gitlab.engr.illinois.edu/engrit-epm/org-shared-deployments) | Standardization of MECM collections and deployments across the college | standardization auditing, bulk manipulation, scripting of repetitive processes | Powershell | Public | 
 | [Audit-StaleADComputersInOU](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Audit-StaleADComputersInOU) | Auditing of "stale" AD computer accounts, and bulk remediation | standardization auditing, bulk manipulation, scripting of repetitive processes | Powershell | Private | 
 | [bcdedit-revert-uefi-gpt-boot-order](https://github.com/mmseng/bcdedit-revert-uefi-gpt-boot-order) | Automating the correction of Windows UEFI boot order after installation of Windows modifies it | scripting of repetitive processes | Powershell | Public | 
 | [Compare-AssignmentRevisions](https://gitlab.engr.illinois.edu/engrit-epm/compare-assignmentrevisions) | Collects MECM client data directly from mass endpoints for analysis to identify issues related to deployment bugs in MECM | auditing, info gathering/reporting | Powershell | Public | 
 | [count-ad-objects](https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/count-ad-objects.ps1) | Identify whether a computer already exists in AD for the purposes of using logic in an MECM task sequence | validation | Powershell | Public | 
 | [Covidize-LabOU](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Covidize-LabOU) | Automation of refactoring AD OUs and GPOs to facilitate segregated remote access for COVID remote work purposes | scripting of repetitive processes | Powershell | Private | 
 | [force-mecm-baseline-evaluation](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/force-mecm-baseline-evaluation) | Force the local MECM client (or a list of remote MECM clients) to re-evaluate assignments. Credit goes to UIUC Endpoint Services (EPS) team. | workaround | Powershell | Private | 
 | [force-software-center-assignment-evaluation](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/force-software-center-assignment-evaluation) | Force a list of remote MECM client to re-evaluate their configuration baselines | workaround | Powershell | Private | 
 | [Export-PrintServerPrinters](https://gitlab.engr.illinois.edu/engrit-epm/export-printserverprinters) | Grabs printer data from our print servers, and dumps it to a CSV format, suitable for consumption by my PrinterStatus webtool (mentioned below). | automation, info gathering/reporting | Powershell | Public | 
 | [Get-AppSupersedence](https://gitlab.engr.illinois.edu/engrit-epm/get-appsupersedence) | Analyzes data from MECM to identify mis-configured application packages, which cause deployment issues | auditing, info gathering/reporting | Powershell | Public | 
 | [Get-CobblerSystems](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-CobblerSystems) | Retrieve all Linux system information from Cobbler instance | info gathering/reporting | Powershell | Private | 
 | [Get-SccmEngrPrefixes](https://gitlab.engr.illinois.edu/engrit-epm/get-sccmengrprefixes) | Retrieve all ENGR computer name prefixes used by MECM to determine which unit's All-Systems collection should receive newly imported computer objects | info gathering/reporting | Powershell | Public | 
 | [Helptools Importer](https://gitlab.engr.illinois.edu/engrit-epm/helptools-importer) | Web-based tool (leveraging Jenkins) for automation of importing new computer information to AD, MECM, and IPAM | webtool, automation, workflow | Powershell, Jenkins, CSS, Groovy | Private | 
 | [msi-app-uninstall](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/blob/master/msi-app-uninstall/msi-app-uninstall.ps1) | Uninstall MSI-based apps. Designed primarily to blow away BigFix/IEM client installations on endpoints. | scripting of repetitive processes | Powershell | Private | 
 | [Ping-All](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Ping-All) | Asynchronously ping multiple computers. Useful for instantaneously checking the availability of all computers in a given lab | scripting of repetitive processes, info gathering/reporting | Powershell | Private | 
 | [Ping-OverTime](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Ping-OverTime) | Ping a machine continuously, logging when it stops and starts responging. Useful for monitoring up/down status during operations which require reboots | scripting of repetitive processes, info gathering/reporting | Powershell | Private | 
 | [powershell-profile-example](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/powershell-profile-example) | Example of useful code for a powershell profile (specifically stuff I use in mine) | misc | Powershell | Private | 
 | [PrinterStatus](https://helptools.engrit.illinois.edu/tools/printerstatus/) | One-stop-shop web-based status monitoring (leveraging the SNMP protocol) for all of the college's printers | webtool, info gathering/reporting, workflow | PHP, Powershell | Private | 
 | PWResetV2 | Resetting of administrator account passwords as securely as possible without leveraging something like LAPS. Contact for more information. | scripting of repetitive processes | Powershell | Private | 
 | [Report-AMTStatus](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Report-AMTStatus) | Gathers AMT state information from endpoints | scripting of repetitive processes, info gathering/reporting | Powershell | Private | 
 | [Report-ProductVersion](https://gitlab.engr.illinois.edu/engrit-epm/report-productversion) | Directly polls endpoints to identify where certain applications are installed, and what the installed version is | info gathering/reporting | Powershell | Public | 
 | [Validate-Win7ESUCompat](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Validate-Win7ESUCompat) | Auditing readiness of Win7 systems to accept Extended Service Updates (ESUs) | validation, info gathering/reporting | Powershell | Private | 

## Generalized topics which I have at least some experience with, but which don't represent specific code projects
- Misc gathering, reporting, and manipulation of AD, MECM, LENS, and IPAM data
- Using custom GUI input prompts and logic at the beginning of an MECM task sequence
- Kicking off custom scripts after an MECM task sequence has finished and rebooted, to do things that cannot be done during a TS (such as running Windows updates)
- Automation of AMT commands to endpoints via Intel's IntelvPro Powershell module
- Quick functions for various handy, quick and dirty administrative tasks
- Customization of Powershell profile, with automatic import of various modules, such as those mentioned above
- General practice of thorough process logging for scripts for easy troubleshooting and review

## Notes
- By mseng3
