# Terminal Configurations
See instructions to launch configuration below.


## Configure PowerShell

1. Install oh-my-posh onto machine
```
> Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
> irm get.scoop.sh | iex
> scoop install oh-my-posh
> code $PROFILE
> oh-my-posh.exe init pwsh --config "C:\git\terminal\default-theme-1.json" | Invoke-Expression
```
2. Install "agave NF" font from nerdfonts.com
3. Right click PowerShell terminal > Defaults > Font > Select **agave NF**
4. Restart PowerShell

