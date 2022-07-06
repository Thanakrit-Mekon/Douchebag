# MacOS Setup for Developer

## Sudo using TouchID

```
sudo vi /etc/pam.d/sudo
```

Append first line
```
auth       sufficient     pam_tid.so
```

## Install Homebrew

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Powerline 10k setup

**Download & install Nerdfonts**
[https://github.com/romkatv/dotfiles-public/tree/master/.local/share/fonts/NerdFonts](https://github.com/romkatv/dotfiles-public/tree/master/.local/share/fonts/NerdFonts)

> Install Fonts in Font Book built in application


**Install oh-my-zsh**
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

**Install plugins & theme**

zsh-autosuggestions
```
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions
```

zsh-syntax-highlighting
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting
```

install powerline10k theme
```
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```
> sudo vi ~/.zshrc
> Edit these line
> 
> ZSH_THEME="powerlevel10k/powerlevel10k"
> ENABLE_CORRECTION=“true”
> plugins=(git node npm yarn vscode zsh-autosuggestions zsh-syntax-highlighting)

## ** In any terminal set fonts to nerdfonts to use powerline10k **
