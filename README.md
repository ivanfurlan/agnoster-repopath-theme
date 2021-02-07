# agnoster-repopath.zsh-theme
Custom theme based on https://github.com/agnoster/agnoster-zsh-theme and https://github.com/ChesterYue/ohmyzsh-theme-passion

## Features
- Inside a repository (git or mercurial) show repo's name and the path only from root directory (where there is .git or .hg)
- Show current time in prompt
- After each command show the time cost

## Installation 
**Download theme**
```shell
git clone https://github.com/ivanfurlan/agnoster-repopath-theme.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/agnoster-repopath
```

**Create link for zsh**
```shell
ln -P ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/agnoster-repopath/agnoster-repopath.zsh-theme ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/agnoster-repopath.zsh-theme
```

**Create a backup of .zshrc**
```shell
cp ~/.zshrc ~/.zshrc-bk
```

**Set theme**
```shell
sed -i 's/ZSH_THEME=".*"/ZSH_THEME="agnoster-repopath"/1' ~/.zshrc
```

## Installation with one command
```shell
git clone https://github.com/ivanfurlan/agnoster-repopath-theme.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/agnoster-repopath && ln -P ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/agnoster-repopath/agnoster-repopath.zsh-theme ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/agnoster-repopath.zsh-theme && cp ~/.zshrc ~/.zshrc-bk && sed -i 's/ZSH_THEME=".*"/ZSH_THEME="agnoster-repopath"/1' ~/.zshrc
```
## Plugins that I use
```
plugins=(git vscode node docker python copyfile gitignore mercurial mvn sudo command-not-found colored-man-pages zsh-autosuggestions zsh-syntax-highlighting autoupdate)
```

**zsh-autosuggestions**: https://github.com/zsh-users/zsh-autosuggestions

**zsh-syntax-highlighting**: https://github.com/zsh-users/zsh-syntax-highlighting

## Auto update themes and plugins
**autoupdate**: https://github.com/TamCore/autoupdate-oh-my-zsh-plugins
