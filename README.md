# Matt's code compendium

## Me
I've been an IT Pro for higher education since 2007. This is a list of some projects I've done, mostly Powershell-based.  

My Github.com username is mmseng, but the majority of my scripting work is done for the purposes of system administration in my work for Engineering IT Shared Services, in the Grainger College of Engineering at the University of Illinois, where my NetID is mseng3.  

If you wish to contact me about my work, please use the University's Microsoft Teams system to do so. If you can't, then email to my university email will suffice. For now, I will not monitor communications here on GitHub.  

## Access
Currently much of my work is stored on version control systems internal to the college, though eventually it will be slowly migrated to the university's GitHub.com organizations, which is why I've spun up this page/repo, and I'll try to keep it updated with the current locations of my projects.  

If you do not already have access to a project linked below and are interested in getting access, please contact me per the above. Some projects are already public, some are not, so try the links first. For projects hosted on gitlab.engr-illinois.edu, you must sign in there at least once, so that your account will be generated and can be granted access.

## Compendium

<table>
	<tr>
		<th>Name</th>
		<th>Description</th>
		<th>Home</th>
		<th>Type</th>
		<th>Language</th>
		<th>Visibility</th>
		<th>Reviewed for sensitivity</th>
	</tr>
	<tr>
		<td>Recycle-EWSGuestAccounts</td>
		<td>Bulk provisioning and decommissioning of guest AD accounts</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Recycle-EWSGuestAccounts</td>
		<td>bulk manipulation, scripting of repetitive processes</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>create-role-based-ad-accounts-and-groups</td>
		<td>Creation of role-based AD accounts and groups, i.e. for administrative use, research groups, and RSOs</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/create-role-based-ad-accounts-and-groups</td>
		<td>bulk manipulation, scripting of repetitive processes</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>Create-ICTDocClassAccounts</td>
		<td>Bulk creation of guest AD accounts, i.e. for a semesterly community class</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Create-ICTDocClassAccounts</td>
		<td>Bulk manipulation, scripting of repetitive processes</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>get-lens-info</td>
		<td>Gathers data about the local endpoint's MAC from LENS data and saves it in MECM task sequence variables</td>
		<td>https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/get-lens-info.ps1</td>
		<td>info gathering/reporting</td>
		<td>Powershell</td>
		<td>Public</td>
		<td>Yes</td>
	</tr>
	<tr>
		<td>post-to-slack</td>
		<td>Sends a message to a Slack channel</td>
		<td>https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/post-to-slack.ps1</td>
		<td>info gathering/reporting</td>
		<td>Powershell</td>
		<td>Public</td>
		<td>Yes</td>
	</tr>
	<tr>
		<td>post-to-teams</td>
		<td>Sends a message to a MS Teams channel</td>
		<td>https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/post-to-teams.ps1</td>
		<td>info gathering/reporting</td>
		<td>Powershell</td>
		<td>Public</td>
		<td>Yes</td>
	</tr>
	<tr>
		<td>Get-Sessions</td>
		<td>Gets session data from remote endpoints, and returns it in a proper Powershell object</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-Sessions</td>
		<td>info gathering/reporting</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>Get-ComputersBySessionState</td>
		<td>Gets a list of computers which have sessions matching given criteria</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-ComputersBySessionState</td>
		<td>info gathering/reporting</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>Get-Model</td>
		<td>Gets model and other info (WMI Win32_ComputerSystem class) from remote endpoints</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-Model</td>
		<td>info gathering/reporting</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>Get-DiskSpace</td>
		<td>Gets available and free disk space from remote endpoints, caluclates free space %, and highlights endpoints with low free space</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-DiskSpace</td>
		<td>info gathering/reporting</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>Get-UptimeHistory</td>
		<td>Retrieves precise uptime history from a remote endpoint</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-UptimeHistory</td>
		<td>info gathering/reporting</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>misc-handy-powershell-examples</td>
		<td>Long list of misc syntax, cmdlets, and snippets I've found handy over the years</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/misc-handy-powershell-examples</td>
		<td>misc</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>org-shared-deployments</td>
		<td>Standardization of MECM collections and deployments across the college</td>
		<td>https://gitlab.engr.illinois.edu/engrit-epm/org-shared-deployments</td>
		<td>standardization auditing, bulk manipulation, scripting of repetitive processes</td>
		<td>Powershell</td>
		<td>Public</td>
		<td>Yes</td>
	</tr>
	<tr>
		<td>Audit-StaleADComputersInOU</td>
		<td>Auditing of "stale" AD computer accounts, and bulk remediation</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Audit-StaleADComputersInOU</td>
		<td>standardization auditing, bulk manipulation, scripting of repetitive processes</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>bcdedit-revert-uefi-gpt-boot-order</td>
		<td>Automating the correction of Windows UEFI boot order after installation of Windows modifies it</td>
		<td>https://github.com/mmseng/bcdedit-revert-uefi-gpt-boot-order</td>
		<td>scripting of repetitive processes</td>
		<td>Powershell</td>
		<td>Public</td>
		<td>Yes</td>
	</tr>
	<tr>
		<td>Compare-AssignmentRevisions</td>
		<td>Collects MECM client data directly from mass endpoints for analysis to identify issues related to deployment bugs in MECM</td>
		<td>https://gitlab.engr.illinois.edu/engrit-epm/compare-assignmentrevisions</td>
		<td>auditing, info gathering/reporting</td>
		<td>Powershell</td>
		<td>Public</td>
		<td>Yes</td>
	</tr>
	<tr>
		<td>count-ad-objects</td>
		<td>Identify whether a computer already exists in AD for the purposes of using logic in an MECM task sequence</td>
		<td>https://gitlab.engr.illinois.edu/engrit-epm/sccm-ts-scripts/-/blob/master/count-ad-objects.ps1</td>
		<td>validation</td>
		<td>Powershell</td>
		<td>Public</td>
		<td>Yes</td>
	</tr>
	<tr>
		<td>Covidize-LabOU</td>
		<td>Automation of refactoring AD OUs and GPOs to facilitate segregated remote access for COVID remote work purposes</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Covidize-LabOU</td>
		<td>scripting of repetitive processes</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>force-mecm-baseline-evaluation</td>
		<td>Force the local MECM client (or a list of remote MECM clients) to re-evaluate assignments. Credit goes to UIUC Endpoint Services (EPS) team.</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/force-mecm-baseline-evaluation</td>
		<td>workaround</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>force-software-center-assignment-evaluation</td>
		<td>Force a list of remote MECM client to re-evaluate their configuration baselines</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/force-software-center-assignment-evaluation</td>
		<td>workaround</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>Export-PrintServerPrinters</td>
		<td>Grabs printer data from our print servers, and dumps it to a CSV format, suitable for consumption by my PrinterStatus webtool (mentioned below).</td>
		<td>https://gitlab.engr.illinois.edu/engrit-epm/export-printserverprinters</td>
		<td>automation, info gathering/reporting</td>
		<td>Powershell</td>
		<td>Public</td>
		<td>Yes</td>
	</tr>
	<tr>
		<td>Get-AppSupersedence</td>
		<td>Analyzes data from MECM to identify mis-configured application packages, which cause deployment issues</td>
		<td>https://gitlab.engr.illinois.edu/engrit-epm/get-appsupersedence</td>
		<td>auditing, info gathering/reporting</td>
		<td>Powershell</td>
		<td>Public</td>
		<td>Yes</td>
	</tr>
	<tr>
		<td>Get-CobblerSystems</td>
		<td>Retrieve all Linux system information from Cobbler instance</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Get-CobblerSystems</td>
		<td>info gathering/reporting</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>Get-SccmEngrPrefixes</td>
		<td>Retrieve all ENGR computer name prefixes used by MECM to determine which unit's All-Systems collection should receive newly imported computer objects</td>
		<td>https://gitlab.engr.illinois.edu/engrit-epm/get-sccmengrprefixes</td>
		<td>info gathering/reporting</td>
		<td>Powershell</td>
		<td>Public</td>
		<td>Yes</td>
	</tr>
	<tr>
		<td>Helptools Importer</td>
		<td>Web-based tool (leveraging Jenkins) for automation of importing new computer information to AD, MECM, and IPAM</td>
		<td>https://gitlab.engr.illinois.edu/engrit-epm/helptools-importer</td>
		<td>webtool, automation, workflow</td>
		<td>Powershell, Jenkins, CSS, Groovy</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>msi-app-uninstall</td>
		<td>Uninstall MSI-based apps. Designed primarily to blow away BigFix/IEM client installations on endpoints.</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/blob/master/msi-app-uninstall/msi-app-uninstall.ps1</td>
		<td>scripting of repetitive processes</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>Ping-All</td>
		<td>Asynchronously ping multiple computers. Useful for instantaneously checking the availability of all computers in a given lab</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Ping-All</td>
		<td>scripting of repetitive processes, info gathering/reporting</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>Ping-OverTime</td>
		<td>Ping a machine continuously, logging when it stops and starts responging. Useful for monitoring up/down status during operations which require reboots</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Ping-OverTime</td>
		<td>scripting of repetitive processes, info gathering/reporting</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>powershell-profile-example</td>
		<td>Example of useful code for a powershell profile (specifically stuff I use in mine)</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/powershell-profile-example</td>
		<td>misc</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>PrinterStatus</td>
		<td>One-stop-shop web-based status monitoring (leveraging the SNMP protocol) for all of the college's printers</td>
		<td>https://helptools.engrit.illinois.edu/tools/printerstatus/</td>
		<td>webtool, info gathering/reporting, workflow</td>
		<td>PHP, Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>PWResetV2</td>
		<td>Resetting of administrator account passwords as securely as possible without leveraging something like LAPS</td>
		<td>Contact for more information.</td>
		<td>scripting of repetitive processes</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>Report-AMTStatus</td>
		<td>Gathers AMT state information from endpoints</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Report-AMTStatus</td>
		<td>scripting of repetitive processes, info gathering/reporting</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
	<tr>
		<td>Report-ProductVersion</td>
		<td>Directly polls endpoints to identify where certain applications are installed, and what the installed version is</td>
		<td>https://gitlab.engr.illinois.edu/engrit-epm/report-productversion</td>
		<td>info gathering/reporting</td>
		<td>Powershell</td>
		<td>Public</td>
		<td>Yes</td>
	</tr>
	<tr>
		<td>Validate-Win7ESUCompat</td>
		<td>Auditing readiness of Win7 systems to accept Extended Service Updates (ESUs)</td>
		<td>https://gitlab.engr.illinois.edu/oesr/official_engrit_script_repo/-/tree/master/Validate-Win7ESUCompat</td>
		<td>validation, info gathering/reporting</td>
		<td>Powershell</td>
		<td>Private</td>
		<td>No</td>
	</tr>
</table>

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
