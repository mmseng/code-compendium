# Matt's code compendium

## Me
I've been an IT Pro for higher education since 2007. This is a list of some projects I've done, mostly Powershell-based.  

My Github.com username is mmseng, but the majority of my scripting work is done for the purposes of system administration in my work for Engineering IT Shared Services, in the Grainger College of Engineering at the University of Illinois, where my NetID is mseng3.  

If you wish to contact me about my work, please use the University's Microsoft Teams system to do so. If you can't, then email to my university email will suffice. For now, I will not monitor communications here on GitHub.  

## Access
Currently much of my work is stored on version control systems internal to the college, though eventually it will be slowly migrated to the university's GitHub.com organizations, which is why I've spun up this page/repo, and I'll try to keep it updated with the current locations of my projects.  

If you do not already have access to a project linked below and are interested in getting access, please contact me per the above. Some projects are already public, some are not, so try the links first. For projects hosted on gitlab.engr-illinois.edu, you must sign in there at least once, so that your account will be generated and can be granted access.

## Compendium
The following is a list of the major scripts/modules/projects I've made, roughly organized by their current location and purpose.

 | Description | Home | Type | Language | Visibility | Reviewed for sensitivity | 
 | Bulk provisioning and decommissioning of guest AD accounts | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Recycle-EWSGuestAccounts | bulk manipulation, scripting of repetitive processes | Powershell | Private | No | 
 | Creation of role-based AD accounts and groups, i.e. for administrative use, research groups, and RSOs | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/create-role-based-ad-accounts-and-groups | bulk manipulation, scripting of repetitive processes | Powershell | Private | No | 
 | Bulk creation of guest AD accounts, i.e. for a semesterly community class | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Create-ICTDocClassAccounts | Bulk manipulation, scripting of repetitive processes | Powershell | Private | No | 
 | Gathers data about the local endpoint's MAC from LENS data and saves it in MECM task sequence variables | https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/get-lens-info.ps1 | info gathering/reporting | Powershell | Public | Yes | 
 | Sends a message to a Slack channel | https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/post-to-slack.ps1 | info gathering/reporting | Powershell | Public | Yes | 
 | Sends a message to a MS Teams channel | https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/post-to-teams.ps1 | info gathering/reporting | Powershell | Public | Yes | 
 | Gets session data from remote endpoints, and returns it in a proper Powershell object | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-Sessions | info gathering/reporting | Powershell | Private | No | 
 | Gets a list of computers which have sessions matching given criteria | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-ComputersBySessionState | info gathering/reporting | Powershell | Private | No | 
 | Gets model and other info (WMI Win32_ComputerSystem class) from remote endpoints | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-Model | info gathering/reporting | Powershell | Private | No | 
 | Gets available and free disk space from remote endpoints, caluclates free space %, and highlights endpoints with low free space | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-DiskSpace | info gathering/reporting | Powershell | Private | No | 
 | Retrieves precise uptime history from a remote endpoint | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-UptimeHistory | info gathering/reporting | Powershell | Private | No | 
 | Long list of misc syntax, cmdlets, and snippets I've found handy over the years | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/misc-handy-powershell-examples | misc | Powershell | Private | No | 
 | Standardization of MECM collections and deployments across the college | https://gitlab.engr.illinois.edu/engrit-epm/org-shared-deployments | standardization auditing, bulk manipulation, scripting of repetitive processes | Powershell | Public | Yes | 
 | Auditing of "stale" AD computer accounts, and bulk remediation | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Audit-StaleADComputersInOU | standardization auditing, bulk manipulation, scripting of repetitive processes | Powershell | Private | No | 
 | Automating the correction of Windows UEFI boot order after installation of Windows modifies it | https://github.com/mmseng/bcdedit-revert-uefi-gpt-boot-order | scripting of repetitive processes | Powershell | Public | Yes | 
 | Collects MECM client data directly from mass endpoints for analysis to identify issues related to deployment bugs in MECM | https://gitlab.engr.illinois.edu/engrit-epm/compare-assignmentrevisions | auditing, info gathering/reporting | Powershell | Public | Yes | 
 | Identify whether a computer already exists in AD for the purposes of using logic in an MECM task sequence | https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/count-ad-objects.ps1 | validation | Powershell | Public | Yes | 
 | Automation of refactoring AD OUs and GPOs to facilitate segregated remote access for COVID remote work purposes | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Covidize-LabOU | scripting of repetitive processes | Powershell | Private | No | 
 | Force the local MECM client (or a list of remote MECM clients) to re-evaluate assignments. Credit goes to UIUC Endpoint Services (EPS) team. | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/force-mecm-baseline-evaluation | workaround | Powershell | Private | No | 
 | Force a list of remote MECM client to re-evaluate their configuration baselines | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/force-software-center-assignment-evaluation | workaround | Powershell | Private | No | 
 | Grabs printer data from our print servers, and dumps it to a CSV format, suitable for consumption by my PrinterStatus webtool (mentioned below). | https://gitlab.engr.illinois.edu/engrit-epm/export-printserverprinters | automation, info gathering/reporting | Powershell | Public | Yes | 
 | Analyzes data from MECM to identify mis-configured application packages, which cause deployment issues | https://gitlab.engr.illinois.edu/engrit-epm/get-appsupersedence | auditing, info gathering/reporting | Powershell | Public | Yes | 
 | Retrieve all Linux system information from Cobbler instance | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-CobblerSystems | info gathering/reporting | Powershell | Private | No | 
 | Retrieve all ENGR computer name prefixes used by MECM to determine which unit's All-Systems collection should receive newly imported computer objects | https://gitlab.engr.illinois.edu/engrit-epm/get-sccmengrprefixes | info gathering/reporting | Powershell | Public | Yes | 
 | Web-based tool (leveraging Jenkins) for automation of importing new computer information to AD, MECM, and IPAM | https://gitlab.engr.illinois.edu/engrit-epm/helptools-importer | webtool, automation, workflow | Powershell, Jenkins, CSS, Groovy | Private | No | 
 | Uninstall MSI-based apps. Designed primarily to blow away BigFix/IEM client installations on endpoints. | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/blob/master/msi-app-uninstall/msi-app-uninstall.ps1 | scripting of repetitive processes | Powershell | Private | No | 
 | Asynchronously ping multiple computers. Useful for instantaneously checking the availability of all computers in a given lab | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Ping-All | scripting of repetitive processes, info gathering/reporting | Powershell | Private | No | 
 | Ping a machine continuously, logging when it stops and starts responging. Useful for monitoring up/down status during operations which require reboots | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Ping-OverTime | scripting of repetitive processes, info gathering/reporting | Powershell | Private | No | 
 | Example of useful code for a powershell profile (specifically stuff I use in mine) | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/powershell-profile-example | misc | Powershell | Private | No | 
 | One-stop-shop web-based status monitoring (leveraging the SNMP protocol) for all of the college's printers | https://helptools.engrit.illinois.edu/tools/printerstatus/ | webtool, info gathering/reporting, workflow | PHP, Powershell | Private | No | 
 | Resetting of administrator account passwords as securely as possible without leveraging something like LAPS | Contact for more information. | scripting of repetitive processes | Powershell | Private | No | 
 | Gathers AMT state information from endpoints | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Report-AMTStatus | scripting of repetitive processes, info gathering/reporting | Powershell | Private | No | 
 | Directly polls endpoints to identify where certain applications are installed, and what the installed version is | https://gitlab.engr.illinois.edu/engrit-epm/report-productversion | info gathering/reporting | Powershell | Public | Yes | 
 | Auditing readiness of Win7 systems to accept Extended Service Updates (ESUs) | https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Validate-Win7ESUCompat | validation, info gathering/reporting | Powershell | Private | No |

## Generalized topics which I have at least some experience with, but which don't represent specific code projects
- Misc gathering, reporting, and manipulation of AD, MECM, LENS, and IPAM data
- Using custom GUI input prompts and logic at the beginning of an MECM task sequence
- Kicking off custom scripts after an MECM task sequence has finished and rebooted, to do things that cannot be done during a TS
- Automation of AMT commands to endpoints via Intel's IntelvPro Powershell module
- Quick functions for various handy, quick and dirty administrative tasks
- Customization of Powershell profile, with automatic import of various modules, such as those mentioned above
- General practice of thorough process logging for scripts for easy troubleshooting and review

## Notes
- By mseng3
