# DOTFILE-WINDOWS

## A submodule for dotfiles repo (http://github.com/Zandler/dotfiles)

This repo contains all my config files for windows 11. The most significant thing is cannot need local admin rigths.

Enjoy


### Requirements

- Windows 11 (recomended a clean environment)
- Powershell > 5


### Instructions 

1. Update yout system
2. Execute command thi command. (NOTE: No need local admin)

```powershell

Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
Iwr -Uri https://raw.githubusercontent.com/banco-bmg/dotfiles-windows/refs/heads/main/install.ps1 -OutFile install.ps1; ./install.ps1

```

This script:
- Install scoop
- Install git
- Clone this repo
- Execute bootstrap.ps1
  - Config environment
  - Install some default apps like vscode, power toys, dotnet 
  - **IF** ONLY IF you are local admin, install wsl with Ubuntu


That's it!

