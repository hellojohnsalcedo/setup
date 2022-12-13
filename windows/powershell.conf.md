# Powershell Config
## All configurations are organized under ~/.config/powershell
```
// .config/powershell/user_profile.ps1

Set-Alias vim nvim
```

## Import from organized configuration source to default configuration source
```
// C:\Users\hello\Documents\PowerShell\Microsoft.PowerShell_profile.ps1
nvim $PROFILE 

// default configuration source
. $env:USERPROFILE\.config\powershell\user_profile.ps1
```
