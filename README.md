# SlackExtract
A PowerShell script to extract all messages and files from a User's slack account. Or, optionally specify a limited number of channels to download from.

## From Windows command line enter powershell with scripts enabled:

```powershell -exec bypass```

## Import the Module:

```Import-Module .\SlackExtract.ps1```

## Read Usage Instructions:

 ```Get-Help Invoke-SlackExtract -full```

**Note you will need to login to slack with a Browser and grab the Slack session cookie (the cookie is named "d") and provide it to this script (the script does not utilize the normal credentials)

See the Wiki for additional notes.