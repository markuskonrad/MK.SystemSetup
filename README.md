# System Setup Guide

This guide explains the setup and the tools I use currently for my daily business.
Goal was to have a simple step by step guide on a system refresh.

* Set windows to `Dark` Mode (Colors --> Choose your color --> Dark)
* Set "View --> File name extensions" to `True`
* Set Textsize to `100%` (Rightclick at Desktop --> Displaysettings - Change the size of text, apps, and other items --> 100%)
* Install Chrome
  * Import profiles from `userfolder\Synology\Home\Profiles\Chrome\Bookmarks`
  * Relevant Profiles `Markus`, `ACN`
* Install Firefox
* Outlook
  * Set Timezones (Settings --> Calendar --> Timezones)
    * `GE` - `UTC+01:00`
    * `IN` - `UTC+05:30`
    * `RO` - `UTC+02:00`
  * Deactivate Automatic Mark as Read (Settings --> Mail --> Outlook panes --> Reading Pane... --> Uncheck all boxes)
  * Remove feature bar on right hand side (Click small hand-button in the Quick Access Bar to switch to Mouse Mode - [Link](<https://answers.microsoft.com/en-us/msoffice/forum/all/outlook-the-pop-out-button-is-missing/1b13d713-15db-4e8d-9e4a-004f5e22a089>))
  * Set spacing  [Link](<https://support.microsoft.com/en-us/office/prefer-tighter-spacing-7aedcfaf-03de-49ad-9bf8-8730134f1f3b?ui=en-us&rs=en-us&ad=us>)
  * Enabled Calendar Weeks (Options --> Calendar --> Display Options --> Set "Show week numbers in the month view and the DAte Navigator" to `True`)
* Install Visio Professional
* Install MS Project (Optional since DevOps Sync not working anymore)
* Install Notepad++ ([Link](<https://notepad-plus-plus.org/downloads/>)) in English
* Setup GMail on Chrome
* SignIn to Teams
* Install GitExtensions ([Link](<https://github.com/gitextensions/gitextensions>) - Scroll down on Tag-Page)
  * Confirue all setting (green)
  * Set merge and diff tools (...vsversion/Enterprise/Common7/IDE/devenv.exe)
  * Setup git ssh keys (copy from old system ...user\.ssh)
* Setup GIT for windows (Part of GitExtensions) - Use Notepad++ as default editor
* Clone required GIT repos to `C:\git`
* AutoHotKey
  * Clone `MK.AutoHotKey.git` and run `default.ahk`
  * Install AutoHotKey ([Link](<https://www.autohotkey.com/>))
  * Register `default.ahk` on startup ([Link](<https://www.maketecheasier.com/schedule-autohotkey-startup-windows/>))
* Install latest version of Visual Studio (e.g. 2019 Enterprise)
  * Set Color Theme "Dark"
  * Track Active Item in Solution Explorer `True`
  * Show pinned tabs in a separate row
* Install Synology Drive (Documents and Home)
  * Create Folders
    * C:\Users\markus.konrad\Synology\Home
    * C:\Users\markus.konrad\Synology\Team
  * Uncheck "Create new SynologyDrive Folder"
  * Add Sync Actions
    * /home/Drive/ --> C:\Users\markus.konrad\SynologyDrive\Home [All except Moments]
    * /document --> C:\Users\markus.konrad\Synology\Team
    * "Local Sync-Folder" --> Maybe later
  * Set Notifications to `False`
* Putty
  * Export Registry Settings for Putty from previous system and import at new system ([Link](https://stackoverflow.com/questions/13023920/how-to-export-import-putty-sessions-list))
  * Install Putty (config comes from Registry)
* Install and setup WinSCP - Sessions should come with Putty restore of Registry (Optional, only if required at current engagement)
* Import Firefox Bookmarks from Backup (`userfolder\Synology\Home\Profiles\Firefox`)
* Import Chrome Bookmarks from Backup (`userfolder\Synology\Home\Profiles\Chrome`)
* Import IE Bookmarks from Backup (`userfolder\Synology\Home\Profiles\IE`)
* Copy Firefox profile scripts to the Desktop (userfolder\Synology\Home\Profiles\Firefox)
* Use KeePass from Synology Drive folder (`userfolder\Synology\Home\Tools\KeePass-2.20.1`)
* Setup DCS VPN ([Link Internal](https://dcshelp.service-now.com/nav_to.do?uri=%2Fkb_view.do%3Fsysparm_article%3DKB0090542))
* Install latest .NET Framework DevKit
* Install and activate Screenpresso
  * Set Screenpresso storage folder to `OneDrive\Pics` and the limit to `500` files
  * Set "Show quick capture window" to `False`
* Install and setup Remote Desktop Manager (RDCMan) from Synology Tools folder
* Install MS Terminal
* Set Execution Policy in PowerShell `Set-ExecutionPolicy Unrestricted -Scope CurrentUser`
* Install poshgit - ([Link Download](<https://www.powershellgallery.com/packages/posh-git>) / [Link Setup](<https://github.com/dahlbyk/posh-git>) - Some Powershell commands to be executed)
* Install oh-my-posh - ([Link Download](<https://github.com/JanDeDobbeleer/oh-my-posh>))
* Set PowerShell profile to the new Theme of oh-my-posh running `notepad $PROFILE` and adding 3 lines (see also [PowerShell/Microsoft.PowerShell_profile.ps1](PowerShell/Microsoft.PowerShell_profile.ps1) for more details)
  * `Import-Module posh-git`
  * `Import-Module oh-my-posh`
  * `Set-Theme Paradox`
* Install powerline-fonts to enable the special icons in the prompt bar showing GIT status etc. ([Link Download](<https://github.com/powerline/fonts>))
* Open Powershell settings via UI and select `Font --> DejaVu Sans Mono for Powerline`
* Open MS Terminal settings and update settings according to the profiles.json file in WindowsTerminal folder ([WindowsTerminal/profiles.json](WindowsTerminal/profiles.json), [Link](<https://www.hanselman.com/blog/HowToMakeAPrettyPromptInWindowsTerminalWithPowerlineNerdFontsCascadiaCodeWSLAndOhmyposh.aspx>))
* Visual Studio Code
  * Install Visual Studio Code (Incl. File and Context Menu setting to `True`)
  * Install Extensions for Visual Studio Code
    * `C#`
    * `Azure Repos`
    * `Debugger for Chrome`
    * `Power Shell`
    * `Python`
    * `markdownlint`
    * `Docker`
    * `GitLens`
* Install ThinkCell for PowerPoint ([Link Internal](https://ts.accenture.com/sites/QuickPresentationToolkit/tcdl/default.aspx ))
* Filezilla
  * Run Filezilla from (`userfolder\Synology\Home\Tools\FileZilla-<version>`)
  * Import Filezilla profile from Backup (`userfolder\Synology\Home\Profiles\Filezilla`)
* Install VLC ([Link](https://www.videolan.org/vlc/index.de.html))
* Add Synology as Network Drive in QuickAccess
* Install Postman App ([Link](https://www.getpostman.com/downloads/))
* Setup Printer (Printers and Scanners --> Add --> Select the printer --> Add device)
* Install Docker for Windows ([Link](https://www.docker.com/products/docker-desktop)) and restart which triggers the  Hyper-V installation
* Install Fiddler ([Link](https://www.telerik.com/fiddler))
* Install Adobe Acrobat Reader DC (**Note:** Make sure all checkboxes like Virus Scan trial etc. are disabled before download!)
* Install Azure DevOps Integration for Excel-TFS/AzureDevOps connection ([Link Download](<https://visualstudio.microsoft.com/de/downloads/?q=Office+Integration&rr=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Fazure%2Fdevops%2Fboards%2Fbacklogs%2Foffice%2Ftrack-work%3Fview%3Dazure-devops>))
* Install Paint dot NET Free Version ([Link Download](<https://www.getpaint.net/download.html>))
* Install Python ([Link Download](<https://www.python.org/>)) and set path to `True`
* Install Synology Note Station ([Link Download](<https://www.synology.com/de-de/support/download/DS716+II#utilities>))
* Install Node.js without tools ([Link Download](<https://nodejs.org/en/download/>))
* Install WSL via 'Turn Windows features on or off'
  * Windows Subsystem for Linux
  * Virtual Machine Platform
* Install Ubuntu via Store
* Set up Tethering
* Set up SSRS Reporting Environment for D365 (Status 2019-12-02) - (Optional, only if required at current engagement)
  * Install Visual Studio 2015 Enterprise in English
  * Install SQL Server Data Tools (SSDT) in English ([Link Download](<https://docs.microsoft.com/en-us/previous-versions/mt186501(v=msdn.10)?redirectedfrom=MSDN>))
  * Install Microsoft Dynamics 365 Report Authoring Extensions ([Link Download](<https://www.microsoft.com/en-us/download/confirmation.aspx?id=50375>))
* Install Adobe Flash (For cam´s only)
* Install 7-Zip ([Link Download](<https://7-zip.de/download.html>))
* Install Streamdeck
  * Backup via Synology folder Tools\Streamdeck
* Install Slack (Optional, only if required at current engagement. Otherwise browser only)
* Setup Home VPN
* Install Logitech Drivers/Tools
* Dump C-Backups to new environment
* Install Azure Storage Explorer
