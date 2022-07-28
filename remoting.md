To enable remote desktop on a PC open a PowerShell Window and set the fDenyTSConnections property on Remote Desktop Registry key to 0:
```ps1
$regKey = "HKLM:\SYSTEM\CurrentControlSet\Control\Terminal Server"
Set-ItemProperty $regKey fdenyTSConnections 0
```

To enable PowerShell Remoting simply run the following within PowerShell:

```ps1
Enable-PSRemoting
```
