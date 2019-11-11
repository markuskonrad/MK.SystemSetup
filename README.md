# System Setup Guide

This guide explains the setup and the tools I use currently for my daily business.
Goal was to have a simple step by step guide on a system refresh.

* Set windows to `Dark` Mode (Colors --> Choose your color --> Dark)
* Set Textsize to `100%` (Rightclick at Desktop --> Displaysettings - Change the size of text, apps, and other items --> 100%)
* Install Chrome
* Install Firefox
* Install latest version of Visual Studio (e.g. 2019 Enterprise)
* Outlook
  * Set Timezones (Settings --> Calendar --> Timezones)
    * `GE` - `UTC+01:00`
    * `IN` - `UTC+05:30`
    * `RO` - `UTC+02:00`
  * Deactivate Automatic Mark as Read (Settings --> Mail --> Outlook panes --> Reading Pane... --> Uncheck all boxes)
  * Remove feature bar on right hand side (Click small hand-button in the Quick Access Bar to switch to Mouse Mode - [Link](<https://answers.microsoft.com/en-us/msoffice/forum/all/outlook-the-pop-out-button-is-missing/1b13d713-15db-4e8d-9e4a-004f5e22a089>))
* Install Visio
* Install MS Project
* Install Notepad++ ([Link](<https://notepad-plus-plus.org/downloads/>))
* Setup GMail on Firefox
* SignIn to Teams
* Setup GIT for windows (Part of GitExtensions) - Use Notepad++ as default editor
* Install GitExtensions ([Link](<https://github.com/gitextensions/gitextensions>) - Scroll down on Tag-Page)
* Clone required GIT repos to `C:\git`
* Install AutoHotKey ([Link](<https://www.autohotkey.com/>))
* Clone `MK.AutoHotKey.git` and run `default.ahk`
* Register `default.ahk` on startup ([Link](<https://www.maketecheasier.com/schedule-autohotkey-startup-windows/>))
* Install Synology Drive (Documents and Home)
* Export Registry Settings for Putty from previous system and import at new system ([Link](https://stackoverflow.com/questions/13023920/how-to-export-import-putty-sessions-list))
* Install Putty (config comes from Registry)
* Install and setup WinSCP - Sessions should come with Putty restore of Registry
* Import Firefox Bookmarks from Backup (`userfolder\Synology\Home\Profiles\Firefox`)
* Import Chrome Bookmarks from Backup (`userfolder\Synology\Home\Profiles\Chrome`)
* Import IE Bookmarks from Backup (`userfolder\Synology\Home\Profiles\IE`)
* Copy Firefox profile scripts to the Desktop (userfolder\Synology\Home\Profiles\Firefox)
* Use KeePass from Synology Drive folder (`userfolder\Synology\Home\Tools\KeePass-2.20.1`)
* Setup DCS VPN ([Link Internal](https://dcshelp.service-now.com/nav_to.do?uri=%2Fkb_view.do%3Fsysparm_article%3DKB0090542))
* Install latest .NET Framework DevKit
* Install and activate Screenpresso
* Set Screenpresso storage folder to `OneDrive\Pics` and the limit to `500` files
* Install and setup Remote Desktop Manager (RDCMan)
* Install MS Terminal
* Install poshgit - ([Link Download](<https://www.powershellgallery.com/packages/posh-git>) / [Link Setup](<https://github.com/dahlbyk/posh-git>) - Some Powershell commands to be executed)
* Install Visual Studio Code (Incl. File and Context Menu setting to `true`)
* Install Extensions for Visual Studio Code
  * `C#`
  * `Azure Repos`
  * `Debugger for Chrome`
  * `Power Shell`
  * `Python`
  * `markdownlint`
  * `Docker`
* Install ThinkCell for PowerPoint ([Link Internal](https://ts.accenture.com/sites/QuickPresentationToolkit/tcdl/default.aspx ))
* Run Filezilla from (`userfolder\Synology\Home\Tools\FileZilla-<version>`)
* Import Filezilla profile from Backup (`userfolder\Synology\Home\Profiles\Firefox`)
* Install VLC ([Link](https://www.videolan.org/vlc/index.de.html))
* Add Synology as Network Drive in QuickAccess
* Install Postman App ([Link](https://www.getpostman.com/downloads/))
* Setup Printer (Printers and Scanners --> Add --> Select the printer --> Add device)
* Install Docker for Windows ([Link](https://www.docker.com/products/docker-desktop)) and restart which triggers the  Hyper-V installation
* Install Fiddler ([Link](https://www.telerik.com/fiddler))
* Install Adobe Acrobat Reader DC (**Note:** Make sure all checkboxes like Virus Scan trial etc. are disabled before download!)
