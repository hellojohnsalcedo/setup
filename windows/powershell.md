# Powershell Recipes

## Directory structure
```
$env:USERPROFILE\.config
  └─ powershell
    └─ user_profile.ps1
    └─ my.omp.json
```

## Package Managers (App Installers)
### Scoop
See [home](https://scoop.sh/)

### Chocolatey
See [home](https://chocolatey.org/)

### winget
Winget is the default App Installer for Windows. For more info, see [docs](https://learn.microsoft.com/en-us/windows/package-manager/winget/).

## How do I get multiple tabs on the terminal
### Links
- [Microsoft Terminal](https://github.com/microsoft/terminal)


## How do I print env on Powershell
### Tokens
```
env:
Get-ChildItem
  └─ aliases
    └─ gci
    └─ dir
    └─ ls
```

## How do I create a file on Powershell
### Tokens
```
$null
  └─ $null > filename
  └─ $null | sc filename
New-Item
  └─ ni filename
```

## How do I print Powershell version
### Tokens
```
$PSVersionTable
```

### Example
```
PS C:\Users\hello> $PSVersionTable

Name                           Value
----                           -----
PSVersion                      5.1.22000.832
PSEdition                      Desktop
PSCompatibleVersions           {1.0, 2.0, 3.0, 4.0...}
BuildVersion                   10.0.22000.832
CLRVersion                     4.0.30319.42000
WSManStackVersion              3.0
PSRemotingProtocolVersion      2.3
SerializationVersion           1.1.0.1
```

## How do I install CLI applications
### References
See [package managers](#package-managers)

### Tokens
```
winget
  └─ search
    └─ Microsoft.PowerShell
  └─ install
    └─ --id Microsoft.PowerShell --source winget
```

## How do I find files
### References
[Use windows powershell to search for files](https://devblogs.microsoft.com/scripting/use-windows-powershell-to-search-for-files/)
