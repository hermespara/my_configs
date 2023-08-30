# my_configs

Notes for future me in case I need to configurate my new PC

## Install `R`

Check out the website ![https://cloud.r-project.org/](https://cloud.r-project.org/)

## Install `R studio`

Download .deb file for the corresponding OS at ![https://posit.co/download/rstudio-desktop/](https://posit.co/download/rstudio-desktop/).

Install rstudio via the terminal:

```
sudo dpkg -i rstudio-{version}-amd64.deb
```

You may need to install `libssl-dev, libclang-dev, libpq5`. 

## Install `Terminator`

A handy terminal:

```
sudo add-apt-repository ppa:gnome-terminator/ppa
sudo apt install terminator
```

Change the following parameters:
1. Terminator separator size to 2
2. In profiles, deselect title bar
3. In command you can add a custom command to run zsh for example `/usr/bin/zsh`
4. In background, add transperency to 0.8-0.9
5. In scrolling check infinite scrollback


## Install `zsh`

```
sudo apt install zsh
```

## Install `oh my zsh`
You'll need
```
sudo apt  install curl
sudo apt install git
```

oh-myzsh
```
wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh
sh install.sh
```

Than powerlevel10k theme:
! do not forget the font installation

```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

Set ZSH_THEME="powerlevel10k/powerlevel10k" in `~/.zshrc`.

plugins: 
```
plugins=(git
	extract
	colored-man-pages
	last-working-dir
	zsh-autosuggestions
	zsh-syntax-highlighting
	z
  git-extra-commands
  zsh-history-substring-search)
```

Install zsh-autosuggestions
```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

syntax highlight
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

git commands plugin

```
git clone https://github.com/unixorn/git-extra-commands.git $ZSH_CUSTOM/plugins/git-extra-commands
```

history substring search

```
 git clone https://github.com/zsh-users/zsh-history-substring-search ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-history-substring-search
```

## JetBrains font

Font for editors ;)

Check out ![https://www.jetbrains.com/fr-fr/lp/mono/#how-to-install](https://www.jetbrains.com/fr-fr/lp/mono/#how-to-install)
