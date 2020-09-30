# Haskell
> Code written in Haskell is guaranteed to have no side effects ... because no one will ever run it? 
> -- *[XKCD 1312](https://www.xkcd.com/1312)*

Haskell recently changed the recommended installation method to include Chocolatey (a Windows package manager), this
seems to be the only way to install the entire platform at the latest version. These instructions are based off
[https://www.haskell.org/platform/windows.html](https://www.haskell.org/platform/windows.html).

1. Install [Chocolatey](https://chocolatey.org/install) using the script below in an administrator PowerShell (right 
click windows terminal and select `run as administrator`).

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

2. Wait for the installation to complete and then run `choco` to check it all works

3. In your administrator PowerShell then run the following two commands:

```powershell
choco install haskell-dev
refreshenv
```

4. Install [Visual Studio Code](https://code.visualstudio.com/) either via Chocolatey or by downloading the installer.

```powershell
choco install vscode
```

5. Once installed, open and go to extensions on the left-hand side (4 squares with one offset) and install
[`Haskelly`](https://marketplace.visualstudio.com/items?itemName=UCL.haskelly) which was written by UCL
Computer Science students to give you pretty syntax highlighting for Haskell in VS Code. Cool, huh?

![Haskelly](../images/windows-haskell-haskelly.png)
