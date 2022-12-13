# Powershell Config
## All configurations are organized under ~/.config/powershell
```
// .config/powershell/user_profile.ps1

Set-Alias vim nvim
```

## Import from organized configuration source to default configuration source
```
nvim ...

// default configuration source
. $env:USERPROFILE\.config\powershell\user_profile.ps1
```
