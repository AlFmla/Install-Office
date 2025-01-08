[![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/Q5Q51QUJC)

## Download Microsoft 365 (Office 365) via ODT with PowerShell 

## How-to

* Download the latest archive and expand it;
* Open PowerShell console as admin and change execution policy

  ```powershell
  Set-ExecutionPolicy -ExecutionPolicy Bypass -Force
  ```

* Open folder in PowerShell console and choose which Office to download

  ```powershell
  .\Download.ps1 -Branch ProPlus2019Retail -Channel Current -Components Word, Excel, PowerPoint
  .\Download.ps1 -Branch ProPlus2021Volume -Channel PerpetualVL2021 -Components Excel, Word
  .\Download.ps1 -Branch ProPlus2024Volume -Channel PerpetualVL2024 -Components Excel, OneDrive, PowerPoint, Word
  .\Download.ps1 -Branch O365ProPlusRetail -Channel Current -Components Excel, OneDrive, Outlook, PowerPoint, Teams, Word
  ```

* Run `.\Install.ps1` from context menu to install Office you downloaded;

## Addendum

`Office 2019, 2021, 2024, & 365` support `Windows 10` & `Windows 11` only

## Features

<details>
  <summary>List</summary>

* General
* Remove diagnostics tracking scheduled tasks
* Do not send additional diagnostic and usage data to Microsoft
* Disable LinkedIn features in Office applications
* Turn off the cloud features
* Turn on Touch/Mouse Mode

* Word
  * Do not show the Start screen when application starts
  * Do not open e-mail attachments and other uneditable files in reading view
  * Disable Protected View for files originating from the Internet
  * Disable Protected View for files located in potentially unsafe locations
  * Disable Protected View for Outlook attachments
  * Show the ruler
  * Save AutoRecover information every 3 minutes
  * Enable the "Draw" tab
  * Enable the "Developer" tab
  * Remove Adobe Acrobat Pro DC COM Add-ins

* Excel
  * Do not show the Start screen when application starts
  * Disable Protected View for files originating from the Internet
  * Disable Protected View for files located in potentially unsafe locations
  * Disable Protected View for Outlook attachments
  * Save AutoRecover information every 3 minutes
  * Enable the "Draw" tab
  * Enable the "Developer" tab

</details>

## Links

* [Configure Office](https://config.office.com/deploymentsettings)
* Overview of update channels
  * <https://learn.microsoft.com/en-us/deployoffice/overview-update-channels>
  * <https://learn.microsoft.com/en-us/microsoft-365/troubleshoot/installation/product-ids-supported-office-deployment-click-to-run>
* [Office Deployment Tool](https://www.microsoft.com/en-us/download/details.aspx?id=49117)
* [Deploy Office](https://learn.microsoft.com/en-us/deployoffice/deployment-guide-microsoft-365-apps)
* [Uninstall Office (SaRA)](https://www.microsoft.com/en-us/download/100607)
* [OffScrubC2R.vbs 2.19](https://github.com/farag2/Office/tree/master/Office_Uninstall)
* [Office Tool Plus](https://github.com/YerongAI/Office-Tool)
