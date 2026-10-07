# Awesome Hardening

 [![Sponsor](https://img.shields.io/badge/Sponsor-Click%20Here-ff69b4)](https://github.com/sponsors/simeononsecurity) 

A collection of scripts, configurations, and tools for hardening various systems and applications.

## Choosing a project

Match the target OS, edition, workload, and recovery procedure before selecting a tool. A repository listing does not establish current platform support or compliance. Check the linked project's current documentation and release history.

The following observations reflect default-branch source reviewed on October 6, 2026. They do not certify runtime compatibility. Check newer releases for repairs after this date.

| Project | Intended use and compatibility scope | Maintenance evidence at review | Recovery evidence at review |
| --- | --- | --- | --- |
| [Windows Optimize Harden Debloat](https://github.com/simeononsecurity/Windows-Optimize-Harden-Debloat) | Windows 10/11 Pro or Enterprise configuration. Broad changes require a disposable test system. | Latest default-branch commit: April 2025. Latest published release: August 2023. | Restore-point code exists. Successful restoration was not verified. |
| [Windows Defender Hardening](https://github.com/simeononsecurity/Windows-Defender-Hardening) | Defender settings on Windows. Confirm available commands and management-policy restrictions. | Latest default-branch commit: December 2024. | No restore operation in reviewed entry script. |
| [AppLocker Hardening](https://github.com/simeononsecurity/Applocker-Hardening) | Application control on systems with AppLocker commands and service support. | Latest default-branch commit: July 2024. | No backup/restore operation in reviewed entry script. |
| [Firefox Privacy Script](https://github.com/simeononsecurity/FireFox-Privacy-Script) | Firefox configuration on Windows, Linux, and macOS. Package layout and ESR variants require testing. | Latest default-branch commit: March 2025. | Uninstall exists. Reviewed shell uninstall removes entire preference/extension directory contents. |
| [Windows Hardening CTF](https://github.com/simeononsecurity/Windows-Hardening-CTF) | Competition and lab systems only. Service shutdown affects remote administration and file sharing. | Latest default-branch commit: July 2024. | No rollback procedure verified. Use a VM snapshot or full backup. |
| [Standalone Windows Server STIG](https://github.com/simeononsecurity/Standalone-Windows-Server-STIG-Script) | README lists Server 2012, 2016, and 2019. Treat newer server support as unverified. | Latest default-branch commit: July 2024. | No restoration workflow verified. Test role and remote-access continuity. |

Commit recency does not establish maintenance quality. Review the source version, unresolved issues, tests, and release contents. For managed systems, check domain or MDM policy precedence. For STIG tooling, verify the exact baseline version and assess each applicable control.

## Windows Hardening

- [Windows Optimize Harden Debloat](https://github.com/simeononsecurity/Windows-Optimize-Harden-Debloat) - Script for optimizing and hardening Windows systems.
- [Windows Optimize Harden Debloat GUI](https://github.com/simeononsecurity/Windows-Optimize-Harden-Debloat-GUI) - GUI version of Windows Optimize Harden Debloat script.
- [Windows Defender Hardening](https://github.com/simeononsecurity/Windows-Defender-Hardening) - Script for hardening Windows Defender.
- [Windows Defender Application Control Hardening](https://github.com/simeononsecurity/Windows-Defender-Application-Control-Hardening) - Script for hardening Windows Defender Application Control.
- [Windows Terminal Hardening](https://github.com/simeononsecurity/Windows-Terminal-Hardening) - Script for hardening Windows Terminal.
- [Applocker Hardening](https://github.com/simeononsecurity/Applocker-Hardening) - Script for hardening Applocker.
- [Windows Hardening CTF](https://github.com/simeononsecurity/Windows-Hardening-CTF) - Competition-only hardening. Disables command access and services including WinRM and SMB. Review scored service requirements before use. Do not treat this script as a general production baseline.
- [Windows Defender Application Guard Hardening](https://github.com/simeononsecurity/Windows-Defender-Application-Guard-Hardening) - Script for hardening Windows Defender Application Guard.
- [Windows STIG Ansible Playbooks](https://github.com/simeononsecurity/Windows_STIG_Ansible) - Ansible playbooks for STIG-compliant Windows systems.
- [Windows Defender STIG Script](https://github.com/simeononsecurity/Windows-Defender-STIG-Script) - Script for STIG-compliant Windows Defender.
- [Standalone Windows Server STIG Script](https://github.com/simeononsecurity/Standalone-Windows-Server-STIG-Script) - Standalone script for STIG-compliant Windows Server.
- [Standalone Windows STIG Script](https://github.com/simeononsecurity/Standalone-Windows-STIG-Script) - Standalone script for STIG-compliant Windows systems.
- [STIG Compliant Domain Prep](https://github.com/simeononsecurity/STIG-Compliant-Domain-Prep)- Script to import STIG compliant GPOs into a domain controller for use in a windows domain environment.
- [HotCakeX/Harden-Windows-Security](https://github.com/HotCakeX/Harden-Windows-Security) - Harden Windows Safely, Securely, with Official Microsoft Methods

## Linux Hardening
- [ansible-collection-hardening](https://github.com/dev-sec/ansible-collection-hardening) - This Ansible collection provides battle tested hardening for Linux, SSH, nginx, MySQL
- [Hardening](https://github.com/konstruktoid/hardening) - Bash Scripts and Ansible Playbooks. Works on Debian and RHEL Based Distros

## VMWare Hardening
- [vmware-stig-powercli](https://github.com/simeononsecurity/vmware-stig-powercli) - PowerCLI Check and Remediation scripts for VMware

## Web Server Hardening
- [Apache Web Server Hardening](https://github.com/simeononsecurity/Apache-Web-Server-Hardening) - Scripts and documentation for hardening Apache Web Server.
- [Dev-Sec.io Hardening Nginx using Ansible](https://github.com/dev-sec/ansible-collection-hardening) - This role provides secure nginx configuration

## Application Hardening
- [.NET STIG Script](https://github.com/simeononsecurity/.NET-STIG-Script) - Script for STIG-compliant .NET applications.
- [Adobe Reader DC STIG Script](https://github.com/simeononsecurity/Adobe-Reader-DC-STIG-Script) - Script for STIG-compliant Adobe Reader DC.
- [Oracle JRE 8 STIG Script](https://github.com/simeononsecurity/Oracle-JRE-8-STIG-Script) -  Script for STIG-compliant Oracle JRE 8.
- [FireFox STIG Script](https://github.com/simeononsecurity/FireFox-STIG-Script) - Script for STIG-compliant FireFox.

## Contributing

For each new entry, include:

- The upstream project and a specific purpose.
- Supported platforms or a clear statement when support is unverified.
- Production, lab, or competition scope.
- A link to installation and recovery instructions, if available.
- Source-review date and supporting maintenance evidence.

Avoid duplicate upstream projects and blanket safety or compliance claims. Report broken links through an issue or pull request. Review redirects before replacing links. Update dated observations only after checking the linked source.

<a href="https://simeononsecurity.ch" target="_blank" rel="noopener noreferrer">
  <h2>Explore the World of Cybersecurity</h2>
</a>
<a href="https://simeononsecurity.ch" target="_blank" rel="noopener noreferrer">
  <img src="https://simeononsecurity.ch/img/banner.png" alt="SimeonOnSecurity Logo" width="300" height="300">
</a>

### Links:
- #### [github.com/simeononsecurity](https://github.com/simeononsecurity)
- #### [simeononsecurity.ch](https://simeononsecurity.ch)

## Learn more about [Hardening Automations and Scripts](https://simeononsecurity.ch/github/awesome-hardening)


