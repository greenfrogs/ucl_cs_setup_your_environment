# Haskell
> Code written in Haskell is guaranteed to have no side effects ... because no one will ever run it? 
> -- *[XKCD 1312](https://www.xkcd.com/1312)*

Haskell recently changed the recommended installation method to installing GHCup. These instructions are based off
[https://www.haskell.org/downloads/](https://www.haskell.org/downloads/).

1. Install GHC, cabal-install, stack and haskell-language-server via GHCupusing the script below:

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force;[System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072;Invoke-Command -ScriptBlock ([ScriptBlock]::Create((Invoke-WebRequest https://www.haskell.org/ghcup/sh/bootstrap-haskell.ps1 -UseBasicParsing))) -ArgumentList $true
```

There's also a [youtube video](https://www.youtube.com/watch?v=bB4fmQiUYPw) explaining installation on windows.

4. Install [Visual Studio Code](https://code.visualstudio.com/).

5. Once installed, open and go to extensions on the left-hand side (4 squares with one offset) and install
[`Haskelly`](https://marketplace.visualstudio.com/items?itemName=UCL.haskelly) which was written by UCL
Computer Science students to give you pretty syntax highlighting for Haskell in VS Code. Cool, huh?

![Haskelly](../images/windows-haskell-haskelly.png)
