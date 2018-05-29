# Einrichtung eines neuen Macs
Hier dokumentiere ich für mich die Einrichtung eines neuen Mac. 

# Tools
## Brew
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

## ZSH
Alternative fish
```
brew install zsh zsh-completion
chsh -s /usr/local/bin/zsh
```

## Oh My Zsh
```
curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh
```
Change the theme
```
git clone https://github.com/dnlkng/oh-my-zsh.git
cp dev/oh-my-zsh/themes/denial.zsh-theme ~/.oh-my-zsh/themes
vim .zshrc
```

## fzf
```
brew install fzf
/usr/local/opt/fzf/install
```
## ripgrep
```
brew install ripgrep
```


## bfs
```
brew install tavianator/tap/bfs
```

## tmux
```
brew install tmux
```

## git
```
git config --global user.email "daniel.koenig@dampsoft.de"
git config --global user.name "könig"
```

## MacVim
```
cd /Applications/MacVim.app/Contents/MacOS
cp Vim /usr/local/bin/mvim
ln -s /usr/local/bin/mvim vim
```

## Vundle
```
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
mvim ~/.vimrc
```

## fd
## zplug
## exa
```
brew install exa
```
## ranger
```
brew install ranger
```
## tldr
```
brew install tldr
```

## Sublime Text 3
```
ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl
```

## iTerm2
### Solarized Dark Theme
