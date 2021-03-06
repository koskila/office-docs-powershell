# Office PowerShell Cmdlet Updater

## Usage:
1. Clone repo at: https://github.com/microsoftdocs/office-docs-powershell
1. Configure your email address in tools/.local/config/default.json to receive emailed logs. (OPTIONAL)
1. Confirm you have NodeJS installed.
    Open PowerShell or GitBash and type `npm --version`. 
    If not, install from [https://nodejs.org/en/download/](https://nodejs.org/en/download/).
1. Open GitBash or PowerShell and cd into office-docs-powershell/tools/office-powershell-updater
1. Install the required modules, type `npm install` and press Enter.
1. Install required PowerShell modules and connectors:
    - Skype for Business Online: https://docs.microsoft.com/en-us/office365/enterprise/powershell/manage-skype-for-business-online-with-office-365-powershell
    - Microsoft Teams:
    - SharePoint Online: 
    - Exchange Online: 
    - Whiteboard: 
    - StaffHub: 
    - Office Online Server: 
    - SharePoint Migration Tool (SPMT):  
1. Run the app, type `npm start` and press Enter.

## Notes
1. The modules are installed from the PowerShell Gallery (PSGallery).
    This gallery contains user submitted code.
    If you would rather not install modules from the PSGallery then you can install the modules manually prior to running the tool.
    If you need to add PSGallery as a trusted source, you can so so with the following command:
    `Set-PSRepository -Name "PSGallery" -InstallationPolicy Trusted`

## Sample Run
