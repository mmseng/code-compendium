# Matt's code compendium

## Me
I've been an IT pro for higher education since 2007. This is a list of some projects I've done, mostly Powershell-based, which I felt are worth sharing for other IT pros.  

My Github.com username is mmseng, but the majority of my scripting work is done for the purposes of system administration for Engineering IT Shared Services, in the Grainger College of Engineering at the University of Illinois, where my NetID is mseng3.  

If you wish to contact me about my work, please use the University's Microsoft Teams system to do so, either directly or through the PowerShell User Group team. If you can't, then my university email will suffice. For now, I will not monitor communications here on GitHub.  

I don't claim that all of the code linked below is perfect; I am mostly self-taught when it comes to Powershell. That being said, I generally try to use the best practices I'm aware of through my CS, IT, and security-conscious background. However I'm equally as happy to receive feedback and pointers about my code as I am to receive questions and share my experience. In general the code below is provided mostly as reference material for other IT pros looking for examples and inspiration.  

## Access
Currently much of my work is stored on version control systems internal to the college, though I am working on migrating it to the university's GitHub.com organizations and made public (where possible), which is why I've spun up this page/repo, and I'll try to keep it updated with the current locations of my projects.  

In the table below, a visibility of `Private` means the code is hosted on Engineering IT's "internal" GitLab service and is only accessible to those specifically granted access. `Public` means the code is accessible to the whole internet. `University` means the code is accessible to any member of any organization belonging to University of Illinois' enterprise-wide GitHub license (i.e. basically any university affiliate).  

If you are interested in getting access to a project which is still private, please contact me per the above. For projects hosted on gitlab.engr-illinois.edu, you must sign in there at least once, so that your account will be generated and can be granted access.  

## Compendium

 | Name and link | Description | Type | Language | Visibility | 
 | ------------- | ----------- | ---- | -------- | ---------- | 
 | [Recycle-EWSGuestAccounts](https://github.com/engrit-illinois/Recycle-EWSGuestAccounts) | Bulk provisioning and decommissioning of guest AD accounts | bulk manipulation, scripting of repetitive processes | Powershell | University | 
 | [create-role-based-ad-accounts-and-groups](https://github.com/engrit-illinois/create-role-based-ad-accounts-and-groups) | Creation of role-based AD accounts and groups, i.e. for administrative use, research groups, and RSOs | bulk manipulation, scripting of repetitive processes | Powershell | University | 
 | [Create-ICTDocClassAccounts](https://github.com/engrit-illinois/Create-ICTDocClassAccounts) | Bulk creation of guest AD accounts, i.e. for a semesterly community class | Bulk manipulation, scripting of repetitive processes | Powershell | University | 
 | [get-lens-info](https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/get-lens-info.ps1) | Gathers data about the local endpoint's MAC from LENS data and saves it in MECM task sequence variables | info gathering/reporting | Powershell | Public | 
 | [post-to-slack](https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/post-to-slack.ps1) | Sends a message to a Slack channel | info gathering/reporting | Powershell | Public | 
 | [post-to-teams](https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/post-to-teams.ps1) | Sends a message to a MS Teams channel | info gathering/reporting | Powershell | Public | 
 | [Get-Sessions](https://github.com/engrit-illinois/Get-Sessions) | Gets session data from remote endpoints, and returns it in a proper Powershell object | info gathering/reporting | Powershell | Public | 
 | [Get-ComputersBySessionState](https://github.com/engrit-illinois/Get-ComputersBySessionState) | Gets a list of computers which have sessions matching given criteria | info gathering/reporting | Powershell | Public | 
 | [Get-Model](https://github.com/engrit-illinois/Get-Model) | Gets model and other info (WMI Win32_ComputerSystem class) from remote endpoints | info gathering/reporting | Powershell | Public | 
 | [Get-DiskSpace](https://github.com/engrit-illinois/Get-DiskSpace) | Gets available and free disk space from remote endpoints, caluclates free space %, and highlights endpoints with low free space | info gathering/reporting | Powershell | Public | 
 | [Get-UptimeHistory](https://github.com/engrit-illinois/Get-UptimeHistory) | Retrieves precise uptime history from a remote endpoint | info gathering/reporting | Powershell | Public | 
 | [Get-FormFactors](https://github.com/engrit-illinois/Get-FormFactors) | Gets form factor and other info (WMI Win32_SystemEnclosure and Win32_ComputerSystem classes) from remote endpoints | info gathering/reporting | Powershell | Public | 
 | [misc-handy-powershell-examples](https://github.com/engrit-illinois/misc-handy-powershell-examples) | Long list of misc syntax, cmdlets, and snippets I've found handy over the years | misc | Powershell | Public | 
 | [org-shared-mecm-deployments](https://github.com/engrit-illinois/org-shared-mecm-deployments) | Standardization of MECM collections and deployments across the college | standardization auditing, bulk manipulation, scripting of repetitive processes | Powershell | Public | 
 | [Audit-StaleADComputersInOU](https://github.com/engrit-illinois/Audit-StaleADComputersInOU) | Auditing of "stale" AD computer accounts, and bulk remediation | standardization auditing, bulk manipulation, scripting of repetitive processes | Powershell | Public | 
 | [bcdedit-revert-uefi-gpt-boot-order](https://github.com/mmseng/bcdedit-revert-uefi-gpt-boot-order) | Automating the correction of Windows UEFI boot order after installation of Windows modifies it | scripting of repetitive processes | Powershell | Public | 
 | [Compare-AssignmentRevisions](https://github.com/engrit-illinois/Compare-AssignmentRevisions) | Collects MECM client data directly from mass endpoints for analysis to identify issues related to deployment bugs in MECM | auditing, info gathering/reporting | Powershell | Public | 
 | [count-ad-objects](https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/count-ad-objects.ps1) | Identify whether a computer already exists in AD for the purposes of using logic in an MECM task sequence | validation | Powershell | Public | 
 | [Covidize-LabOU](https://github.com/engrit-illinois/Covidize-LabOU) | Automation of refactoring AD OUs and GPOs to facilitate segregated remote access for COVID remote work purposes | scripting of repetitive processes | Powershell | Public | 
 | [force-mecm-baseline-evaluation](https://github.com/engrit-illinois/force-mecm-baseline-evaluation) | Force the local MECM client (or a list of remote MECM clients) to re-evaluate assignments. Credit goes to UIUC Endpoint Services (EPS) team. | workaround | Powershell | Public | 
 | [force-software-center-assignment-evaluation](https://github.com/engrit-illinois/force-software-center-assignment-evaluation) | Force a list of remote MECM client to re-evaluate their configuration baselines | workaround | Powershell | Public | 
 | [Get-AppSupersedence](https://github.com/engrit-illinois/Get-AppSupersedence) | Analyzes data from MECM to identify mis-configured application packages, which cause deployment issues | auditing, info gathering/reporting | Powershell | Public | 
 | [Get-CobblerSystems](https://github.com/engrit-illinois/Get-CobblerSystems) | Retrieve all Linux system information from Cobbler instance | info gathering/reporting | Powershell | University | 
 | [Export-LabtrackData](https://github.com/engrit-illinois/Export-LabtrackData) | Retrieve all Windows and Linux system information regarding lab computers from AD and Cobbler and exports to CSV | info gathering/reporting | Powershell | University | 
 | [Get-SccmEngrPrefixes](https://gitlab.engr.illinois.edu/engrit-epm/get-sccmengrprefixes) | Retrieve all ENGR computer name prefixes used by MECM to determine which unit's All-Systems collection should receive newly imported computer objects | info gathering/reporting | Powershell | Public | 
 | [msi-app-uninstall](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/blob/master/msi-app-uninstall/msi-app-uninstall.ps1) | Uninstall MSI-based apps. Designed primarily to blow away BigFix/IEM client installations on endpoints. | scripting of repetitive processes | Powershell | Private | 
 | [Ping-All](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Ping-All) | Asynchronously ping multiple computers. Useful for instantaneously checking the availability of all computers in a given lab | scripting of repetitive processes, info gathering/reporting | Powershell | Public | 
 | [Ping-OverTime](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Ping-OverTime) | Ping a machine continuously, logging when it stops and starts responging. Useful for monitoring up/down status during operations which require reboots | scripting of repetitive processes, info gathering/reporting | Powershell | Private | 
 | [Report-AMTStatus](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Report-AMTStatus) | Gathers AMT state information from endpoints | scripting of repetitive processes, info gathering/reporting | Powershell | Private | 
 | [Report-ProductVersion](https://gitlab.engr.illinois.edu/engrit-epm/report-productversion) | Directly polls endpoints to identify where certain applications are installed, and what the installed version is | info gathering/reporting | Powershell | Public | 
 | [Validate-Win7ESUCompat](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Validate-Win7ESUCompat) | Auditing readiness of Win7 systems to accept Extended Service Updates (ESUs) | validation, info gathering/reporting | Powershell | Private | 
 | [powershell-profile-example](https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/powershell-profile-example) | Example of useful code for a powershell profile (specifically stuff I use in mine) | misc | Powershell | Private | 
 | [Export-PrintServerPrinters](https://github.com/engrit-illinois/Export-PrintServerPrinters) | Grabs printer data from our print servers, and dumps it to a CSV format, suitable for consumption by my PrinterStatus webtool (mentioned below). | automation, info gathering/reporting | Powershell | University | 
 | [PrinterStatus](https://helptools.engrit.illinois.edu/tools/printerstatus/) | One-stop-shop web-based status monitoring (leveraging the SNMP protocol) for all of the college's printers | webtool, info gathering/reporting, workflow | PHP, Powershell | Private | 
 | PWResetV2 | Resetting of administrator account passwords as securely as possible without leveraging something like LAPS. Contact for more information. | scripting of repetitive processes | Powershell | Private | 
 | [Helptools Importer](https://gitlab.engr.illinois.edu/engrit-epm/helptools-importer) | Web-based tool (leveraging Jenkins) for automation of importing new computer information to AD, MECM, and IPAM | webtool, automation, workflow | Powershell, Jenkins, CSS, Groovy | Private | 

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
