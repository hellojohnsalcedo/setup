# Powershell Recipes

## Directory structure
```
$env:USERPROFILE\.config
  └─ powershell
    └─ user_profile.ps1
    └─ my.omp.json
```

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
