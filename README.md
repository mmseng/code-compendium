# Matt's code compendium

## Me and my code
I've been an IT pro for higher education since 2007. This is an index of some projects I've done, mostly Powershell-based, which I felt are worth sharing for other IT pros.  

The majority of my scripting work is done for the purposes of system administration and endpoint management for Engineering IT Shared Services, in the Grainger College of Engineering at the University of Illinois. It focuses on AD, MECM, data gathering and reporting, bulk manipulation, automation of repetitive processes, standardization auditing, and process improvement, with a few custom webtools and integrations thrown in. My GitHub.com username is mmseng, but most of my work is hosted under Engineering IT's university-licensed GitHub.com organization, and attributed to my NetID (mseng3).  

If you wish to contact me about my work, please use the University's Microsoft Teams system to do so, either directly or through the PowerShell User Group team. If you can't, then my university email will suffice. For now, I will not closely monitor communications here on GitHub.  

I don't claim that all of the code linked below is perfect; I am mostly self-taught when it comes to Powershell. That being said, I generally try to use the best practices developed through my CS, IT, and security-conscious background. However I'm equally as happy to receive feedback and pointers about my code as I am to receive questions and share my experience. In general the code below is provided mostly as reference material for other IT pros looking for examples and inspiration.  

The majority of my Powershell code has been developed on v5.1, and most has not been tested on v6 nor v7. However I am using v7 by default now, and try to update or notate code which has issues on versions later than v5.1.  

## Access
Most of this work has been migrated from Engineering's GitLab instance to our GitHub.com university-licensed organization, and has been made public where it makes sense.

In the table below, a visibility of `Public` means the code is accessible to the whole internet. `University` means the code is accessible to any member of any organization belonging to University of Illinois' enterprise-wide GitHub license (i.e. basically any university affiliate, this visiblity is called "Internal" in GitHub.com enterprise parlance). `Private` means the code is still hosted on Engineering IT's GitLab service and is only accessible to those specifically granted access.  

Note:
- For projects hosted on GitHub with a visibility of "University" (a.k.a. "Internal"), you'll need to authenticate your GitHub account via the university SSO, by browsing here: https://github.com/orgs/engrit-illinois/sso.
- If you are interested in getting access to a non-public project, please contact me per the above.

## Compendium
<!-- Table row template
 | [ScriptName](https://github.com/engrit-illinois/ScriptName) | Summary of script | type | Language | Visibility | 
-->

 | Name and link | Description | Type | Language | Visibility | 
 | ------------- | ----------- | ---- | -------- | ---------- | 
 | [how-to-install-a-custom-powershell-module](https://github.com/engrit-illinois/how-to-install-a-custom-powershell-module) | Brief instructions on installing a custom powershell module | informational | English, Powershell | Public | 
 | [how-to-run-custom-powershell-modules-as-another-user](https://github.com/engrit-illinois/how-to-run-custom-powershell-modules-as-another-user) | Instructions referenced by several of my custom modules listed below | informational | English, Powershell | University | 
 | [Get-ClassSize](https://github.com/engrit-illinois/Get-ClassSize) | Returns information about the number of users with the Remote Desktop permission for a given Engineering Instructional lab. | data gathering/reporting | Powershell | University | 
 | [Get-LabRDUCount](https://github.com/engrit-illinois/Get-LabRDUCount) | This is a handy Powershell module for querying the size of a given UIUC Engineering class. | data gathering/reporting | Powershell | University | 
 | [Recycle-EWSGuestAccounts](https://github.com/engrit-illinois/Recycle-EWSGuestAccounts) | Bulk provisioning and decommissioning of guest AD accounts | bulk manipulation, scripting of repetitive processes | Powershell | University | 
 | [Refresh-EWSRDUGroups](https://github.com/engrit-illinois/Refresh-EWSRDUGroups) | Bulk provisioning and decommissioning of AD security groups used to control remote access to EWS labs | bulk manipulation, scripting of repetitive processes | Powershell | University | 
 | [Poke-EwsHomeDir](https://github.com/engrit-illinois/Poke-EwsHomeDir) | Gathers some handy infomation about the Engineering IT EWS home directory for a given user. | data gathering/reporting | Powershell | Private | 
 | [create-role-based-ad-accounts-and-groups](https://github.com/engrit-illinois/create-role-based-ad-accounts-and-groups) | Creation of role-based AD accounts and groups, i.e. for administrative use, research groups, and RSOs | bulk manipulation, scripting of repetitive processes | Powershell | University | 
 | [Create-ICTDocClassAccounts](https://github.com/engrit-illinois/Create-ICTDocClassAccounts) | Bulk creation of guest AD accounts, i.e. for a semesterly community class | Bulk manipulation, scripting of repetitive processes | Powershell | University | 
 | [post-to-slack](https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/post-to-slack.ps1) | Sends a message to a Slack channel | data gathering/reporting | Powershell | Public | 
 | [post-to-teams](https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/post-to-teams.ps1) | Sends a message to a MS Teams channel | data gathering/reporting | Powershell | Public | 
 | [Get-Sessions](https://github.com/engrit-illinois/Get-Sessions) | Gets session data from remote endpoints, and returns it in a proper Powershell object | data gathering/reporting | Powershell | Public | 
 | [get-lens-info](https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/get-lens-info.ps1) | Gathers data about the local endpoint's MAC from LENS data and saves it in MECM task sequence variables | data gathering/reporting | Powershell | Public | 
 | [Get-LensInfo](https://github.com/engrit-illinois/Get-LensInfo) | Retrieves networking info about a given AD computer from the Lens API, and returns it in a proper Powershell object. | data gathering/reporting | Powershell | University |
 | [Get-ComputersBySessionState](https://github.com/engrit-illinois/Get-ComputersBySessionState) | Gets a list of computers which have sessions matching given criteria | data gathering/reporting | Powershell | Public | 
 | [Get-Model](https://github.com/engrit-illinois/Get-Model) | This script reports various inventory-related info from a list of remote computers by polling them asynchronously. | data gathering/reporting | Powershell | Public | 
 | [Get-MachineInfo](https://github.com/engrit-illinois/Get-MachineInfo) | Gets model and other info (WMI Win32_ComputerSystem class) from remote endpoints | data gathering/reporting | Powershell | Public | 
 | [Get-DiskSpace](https://github.com/engrit-illinois/Get-DiskSpace) | Gets available and free disk space from remote endpoints, caluclates free space %, and highlights endpoints with low free space | data gathering/reporting | Powershell | Public | 
 | [Get-MissingDrivers](https://github.com/engrit-illinois/Get-MissingDrivers) | This script asynchronously polls an array of computers and reports whether they have any devices with missing or problematic drivers. | data gathering/reporting | Powershell | Public | 
 | [Get-LocalUserProfiles](https://github.com/engrit-illinois/Get-LocalUserProfiles) | Pulls information about local user profiles from a given array of computers. | auditing, data gathering/reporting | Powershell | Public | 
 | [Remove-LocalUserProfiles](https://github.com/engrit-illinois/Remove-LocalUserProfiles) | Removes local user profiles from a given array of remote computers. | bulk manipulation, scripting of repetitive processes | Powershell | Public | 
 | [Get-UptimeHistory](https://github.com/engrit-illinois/Get-UptimeHistory) | Retrieves precise uptime history from a remote endpoint | data gathering/reporting | Powershell | Public | 
 | [Get-FormFactors](https://github.com/engrit-illinois/Get-FormFactors) | Gets form factor and other info (WMI Win32_SystemEnclosure and Win32_ComputerSystem classes) from remote endpoints | data gathering/reporting | Powershell | Public | 
 | [win7-esu-mecm-baseline](https://github.com/engrit-illinois/win7-esu-mecm-baseline) | A script to be used as a configuration item for a MECM baseline which detects systems with valid Win7 ESUs | data gathering/reporting | Powershell | Public | 
 | [Get-OuLoginMessage](https://github.com/engrit-illinois/Get-OuLoginMessage) | Polls computers in an OU and returns whether they have a login message configured locally. | data gathering/reporting | Powershell | Private | 
 | [misc-handy-powershell-examples](https://github.com/engrit-illinois/misc-handy-powershell-examples) | Long list of misc syntax, cmdlets, and snippets I've found handy over the years | misc | Powershell | Public | 
 | [handy-log-functions](https://github.com/engrit-illinois/handy-log-functions) | Some handy, feature-rich log functions for use in PowerShell modules. | utility | Powershell | Public | 
 | [Get-PsVersion](https://github.com/engrit-illinois/Get-PsVersion) | A hacky PowerShell function to get the PowerShell version of a remote machine. | data gathering/reporting | Powershell | Public | 
 | [org-shared-mecm-deployments](https://github.com/engrit-illinois/org-shared-mecm-deployments) | Standardization of MECM collections and deployments across the college | standardization auditing, bulk manipulation, scripting of repetitive processes | Powershell | Public | 
 | [Get-MacsFromSmsPxeLog](https://github.com/engrit-illinois/Get-MacsFromSmsPxeLog) | Pulls our SMSPXE log from the \\engr-mecmdp-01\logs share and pulls the MACs and some stats, to help identify bootlooping machines. | data gathering/reporting | PowerShell | Public | 
 | [Audit-StaleADComputersInOU](https://github.com/engrit-illinois/Audit-StaleADComputersInOU) | Auditing of "stale" AD computer accounts, and bulk remediation | standardization auditing, bulk manipulation, scripting of repetitive processes | Powershell | Public | 
 | [Audit-MisconfiguredGpos](https://github.com/engrit-illinois/Audit-MisconfiguredGpos) | A script to find GPOs which have no links, or have other potentially undesirable configurations. | data gathering/reporting, auditing | Powershell | Public | 
 | [bcdedit-revert-uefi-gpt-boot-order](https://github.com/mmseng/bcdedit-revert-uefi-gpt-boot-order) | Automating the correction of Windows UEFI boot order after installation of Windows modifies it | scripting of repetitive processes | Powershell | Public | 
 | [Prep-MECM](https://github.com/engrit-illinois/Prep-MECM) | Prepares a connection to MECM so cmdlets from the ConfigurationManager Powershell module can be used. | utility, scripting of repetitive processes | Powershell | University | 
 | [Get-CMAppDepTypeData](https://github.com/engrit-illinois/Get-CMAppDepTypeData) | Script to gather local application deployment type data from remote machines to identify widespread issues | auditing, data gathering/reporting | Powershell | Public | 
 | [Compare-AssignmentRevisions](https://github.com/engrit-illinois/Compare-AssignmentRevisions) | Collects MECM client data directly from mass endpoints for analysis to identify issues related to deployment bugs in MECM | auditing, data gathering/reporting | Powershell | Public | 
 | [Get-AppSupersedence](https://github.com/engrit-illinois/Get-AppSupersedence) | Analyzes data from MECM to identify mis-configured application packages, which cause deployment issues | auditing, data gathering/reporting | Powershell | Public | 
 | [Invoke-TaskSequence](https://github.com/engrit-illinois/Invoke-TaskSequence) | Triggers an MECM Task Sequence on one or more remote computers by communicating directly with their MECM client. | automation | Powershell | Public | 
 | [Get-CMAppFromContentId](https://github.com/engrit-illinois/Get-CMAppFromContentId) | Tries to find the name of the MECM application package associated with a given Content ID. | data gathering/reporting | Powershell | University | 
 | [Get-DeploymentReport](https://github.com/engrit-illinois/Get-DeploymentReport) | Polls SCCM for information about all deployments and exports to a CSV | auditing, data gathering/reporting | Powershell | Public | 
 | [Get-CMCollectionMembersWithAdOus](https://github.com/engrit-illinois/Get-CMCollectionMembersWithAdOus) | Returns all MECM devices in matching collections along with their resource information, including their parent Active Directory OU. | data gathering/reporting | Powershell | University | 
 | [count-ad-objects](https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/count-ad-objects.ps1) | Identify whether a computer already exists in AD for the purposes of using logic in an MECM task sequence | validation | Powershell | Public | 
 | [Covidize-LabOU](https://github.com/engrit-illinois/Covidize-LabOU) | Automation of refactoring AD OUs and GPOs to facilitate segregated remote access for COVID remote work purposes | scripting of repetitive processes | Powershell | Public | 
 | [Get-MembershipOfGroupsInOU](https://github.com/engrit-illinois/Get-MembershipOfGroupsInOU) | This script outputs a CSV file reporting the members of all AD groups found within a given OU. | data gathering/reporting | Powershell | Public | 
 | [Get-ADOUStructureObject](https://github.com/engrit-illinois/Get-ADOUStructureObject) | Takes an OU and prints a visual, textual representation of the OU and it's sub-OUs and computers, retaining the OU structure. | data gathering/reporting | Powershell | Public | 
 | [Remove-AdGroupMemberships](https://github.com/engrit-illinois/Remove-AdGroupMemberships) | A script to remove AD users from AD groups, based on given memberships. | bulk manipulation, scripting of repetitive processes | Powershell | Public | 
 | [Add-AdGroupMemberships](https://github.com/engrit-illinois/Add-AdGroupMemberships) | A script to add AD users to AD groups, based on given memberships. | bulk manipulation, scripting of repetitive processes | Powershell | Public | 
 | [Get-RdcmanFileForOu](https://github.com/engrit-illinois/Get-RdcmanFileForOu) | Outputs an RDG file (for use with RDCMan) with a group structure mimicking the OU structure in a given AD OU. | utility, workaround, scripting of repetitive processes | Powershell | Public | 
 | [force-mecm-baseline-evaluation](https://github.com/engrit-illinois/force-mecm-baseline-evaluation) | Force a list of remote MECM client to re-evaluate their configuration baselines | workaround | Powershell | Public | 
 | [force-software-center-assignment-evaluation](https://github.com/engrit-illinois/force-software-center-assignment-evaluation) | Force the local MECM client (or a list of remote MECM clients) to re-evaluate assignments. Credit goes to UIUC Endpoint Services (EPS) team. | workaround | Powershell | Public | 
 | [Get-CobblerSystems](https://github.com/engrit-illinois/Get-CobblerSystems) | Retrieve all Linux system information from Cobbler instance | data gathering/reporting | Powershell | University | 
 | [Export-LabtrackData](https://github.com/engrit-illinois/Export-LabtrackData) | Retrieve all Windows and Linux system information regarding lab computers from AD and Cobbler and exports to CSV for use in updating the Engineering Labtrack webtool | data gathering/reporting | Powershell | University | 
 | [Get-MecmCollegePrefixes](https://github.com/engrit-illinois/Get-MecmCollegePrefixes) | Retrieve all college computer name prefixes used by your "All Systems" collection to determine which newly imported computer objects to include | data gathering/reporting | Powershell | University | 
 | [remove-pre-2021-autodesk-shortcuts](https://github.com/engrit-illinois/remove-pre-2021-autodesk-shortcuts) | This script blows away all autodesk product shortcuts it can find, except for the 2021 versions | bulk manipulation, workaround | Powershell | Public | 
 | [msi-app-uninstall](https://github.com/engrit-illinois/msi-app-uninstall) | Uninstall MSI-based apps. Designed primarily to blow away BigFix/IEM client installations on endpoints. | scripting of repetitive processes | Powershell | Public | 
 | [New-IpamHostRecord](https://github.com/engrit-illinois/New-IpamHostRecord) | Module for adding a host record to IPAM via the Infoblox WAPI to help with adding multiple records at a time without using the slow web UI, or the convoluted CSV import functionality. | bulk manipulation, scripting of repetitive processes | Powershell | University | 
 | [Set-IpamHostRecord](https://github.com/engrit-illinois/Set-IpamHostRecord) |  Module for modifying host records in IPAM via the Infoblox WAPI to help with editing multiple records at a time without using the slow web UI, or the convoluted CSV import functionality. | type | Language | Visibility | 
 | [Ping-All](https://github.com/engrit-illinois/Ping-All) | Asynchronously ping multiple computers. Useful for instantaneously checking the availability of all computers in a given lab | scripting of repetitive processes, data gathering/reporting | Powershell | Public | 
 | [Ping-OverTime](https://github.com/engrit-illinois/Ping-OverTime) | Ping a machine continuously, logging when it stops and starts responding. Useful for monitoring up/down status during operations which require reboots | scripting of repetitive processes, data gathering/reporting | Powershell | Public | 
 | [Test-DclLabIps](https://github.com/engrit-illinois/Test-DclLabIps) | Quick function to ping the machines in DCL-L416 and DCL-L440 at their AD DNS and regular DNS hostnames, for both their EWS and CBTF builds. | data gathering/reporting | Powershell | Private | 
 | [Report-AMTStatus](https://github.com/engrit-illinois/Report-AMTStatus) | Gathers AMT state information from endpoints | scripting of repetitive processes, data gathering/reporting | Powershell | Public | 
 | [Report-ProductVersion](https://github.com/engrit-illinois/Report-ProductVersion) | Directly polls endpoints to identify where certain applications are installed, and what the installed version is | data gathering/reporting | Powershell | Public | 
 | [Validate-Win7ESUCompat](https://github.com/engrit-illinois/Validate-Win7ESUCompat) | Auditing readiness of Win7 systems to accept Extended Service Updates (ESUs) | validation, data gathering/reporting | Powershell | Public | 
 | [powershell-profile-example](https://github.com/engrit-illinois/powershell-profile-example) | Example of useful code for a powershell profile (specifically stuff I use in mine) | misc | Powershell | University | 
 | [Export-PrintServerPrinters](https://github.com/engrit-illinois/Export-PrintServerPrinters) | Grabs printer data from our print servers, and dumps it to a CSV format, suitable for consumption by my Engineering PrinterStatus webtool (mentioned below). | automation, data gathering/reporting | Powershell | University | 
 | [PrinterStatus](https://helptools.engrit.illinois.edu/tools/printerstatus/) | One-stop-shop web-based status monitoring (leveraging the SNMP protocol) for all of the college's printers | webtool, data gathering/reporting, workflow | PHP, Powershell | Private | 
 | PWResetV2 | Resetting of administrator account passwords as securely as possible without leveraging something like LAPS. Contact for more information. | scripting of repetitive processes | Powershell | Private | 
 | [Helptools Importer](https://gitlab.engr.illinois.edu/engrit-epm/helptools-importer) | Web-based tool (leveraging Jenkins) for automation of importing new computer information to AD, MECM, and IPAM | webtool, automation, workflow | Powershell, Jenkins, CSS, Groovy | Private | 
 | [excel-notes](https://github.com/engrit-illinois/excel-notes) | Just a repository for some handy excel tricks, mostly related to data munging. | data gathering/reporting | Excel | Public | 

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
