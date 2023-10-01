# Terminal Configurations
See instructions to launch configuration below.


## Vim setup
```
> cd "c:\users\YOUR_USERNAME_HERE\AppData\Local\"
> md ~\AppData\Local\nvim\autoload
> $uri = 'https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
    (New-Object Net.WebClient).DownloadFile($uri, $ExecutionContext.SessionState.Path.GetUnresolvedProviderPathFromPSPath("~\AppData\Local\nvim\autoload\plug.vim"))
> Create init.vim in c:\users\YOUR_USERNAME_HERE\AppData\Local\nvim\init.vim
> Edit init.vim to have:
    call plug#begin('~/AppData/Local/nvim/plugged')
    Plug 'catppuccin/nvim', { 'as': 'catppuccin' }
    call plug#end()
> nvim ":PlugInstall"
```
## Configure PowerShell

1. Install oh-my-posh onto machine
```
> Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
> irm get.scoop.sh | iex
> scoop install oh-my-posh
> code $PROFILE
> oh-my-posh.exe init pwsh --config "C:\git\terminal\PowerShell\default-theme-1.json" | Invoke-Expression
```
2. Install "agave NF" font from nerdfonts.com
3. Right click PowerShell terminal > Defaults > Font > Select **Hack Nerd Font** (https://github.com/ryanoasis/nerd-fonts/releases/download/v2.1.0/Hack.zip)
4. Restart PowerShell

