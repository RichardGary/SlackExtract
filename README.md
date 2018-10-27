# SlackExtract
A PowerShell script to extract all messages and files from a User's slack account. Or, optionally specify a limited number of channels to download from.

## From Windows command line enter powershell with scripts enabled:

```powershell -exec bypass```

## Import the Module:

```Import-Module .\SlackExtract.ps1```

## Read Usage Instructions:

 ```Get-Help Invoke-SlackExtract -full```

## Required Parameters

1. SlackUrl (e.g. https://slackextract.slack.com)
2. OutputFolderName (e.g. my-extraction)
3. dCookie (e.g. wvxP...8%3D)   OR   SlackToken (e.g. xoxs-12...65)

## Example 1: Extract all files and messages from each channel (up to the default limits)

### Providing the dCookie

```Invoke-SlackExtract -OutputFolderName my-extraction -SlackUrl https://slackextract.slack.com -dCookie wvxPLsXuW%2BUjT2b5RiCvb%2BUBPlJEX2XWbnVpOTlQZUN1TFF6dkxrNlZJbExYTzN6TmNtdFZNTDY0Y2pVQlF6UXlannhZMkprcHRueE12TVpXaXRvRWtQZGhidlhPdEh2d0J1a0I0UjcxMlRJV2JmTndDMlh1czNlUCt0SWIyczExb0z1ZCtxL3JJRW9tenJFRDhIdmp2MWVIQytLc3Q0RWZLSEFvdTQxUFE9PSy1X4xNmoY5wXzFlw2GJL8%3D```

### Providing the API Token

```Invoke-SlackExtract -OutputFolderName my-extraction -SlackUrl https://slackextract.slack.com -SlackToken xoxs-420083410720-421837374423-440811613314-977844f625b707d5b0b268206dbc92cbc85feef3e71b08e44815a8e6e7657190```

## How to Obtain the dCookie and/or the API Token

## Default Limits

| Limit Parameters        | Default Value   
| :-------------: |:-------------:
| MaxMessagesPerChannel       | 10,000 
| MaxFilesPerChannel     | 2,000      
| MaxUsers  | 100,000
| MaxAccessLogs* | 1000,0000

* Accessible to Admins of Paid Workspaces Only

See the Wiki for additional notes.
