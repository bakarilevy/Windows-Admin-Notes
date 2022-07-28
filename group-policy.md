To add a user to a group from the command line open a PowerShell Window and use the Add-LocalGroupMember cmdlet.
Here is an example of adding a local user to the administrator group, the user account you are using must already be an Administrator:

```ps1
Add-LocalGroupMember -Group "Administrators" -Member "MyAccountName"
```

For more information see the official Microsoft Docs here:

https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.localaccounts/add-localgroupmember?view=powershell-5.1