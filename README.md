# Einrichtung eines neuen Macs
Hier dokumentiere ich für mich die Einrichtung eines neuen Mac. 

# Dotfile Bot
Eventuell sollte ich den [dotfile bot](https://github.com/dnlkng/dotfiles) nutzen

# Tools
## Brew
Homebrew ist der inoffizielle Packagemanager for macOS und eigentlich unersetzlich für Entwickler. Die meisten Packages werden als Source bezogen und lokal gebaut, wobei es auch fertige Binarys gibt.
<https://brew.sh>
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

## ZSH
Ist mächtiger und schneller als Bash oder andere Shells. Ausserdem ist der Community-Support meiner Meinung nach größer.

Als Alternative wäre noch fish zu evaluieren. Wobei diese wohl [keine Posix-Shell](https://stackoverflow.com/questions/48732986/) ist.
```
brew install zsh zsh-completion
chsh -s /usr/local/bin/zsh
```
Die letzte Zeile setzt zsh als Standardshell des Users.

## Oh My Zsh
Hier haben wir ein stark community-getriebenes Framework, um die zsh anzupassen und noch komfortabler zu machen, mit sinnvollen Erweiterungen wie z.B. anpassbare Prompts und vielem mehr. Ich habe allerdings auch schon gelesen, dass oh my zsh zu aufgebläht ist. Daher lohnt es sich eventuell Alternativen wie Prezto und Antigen.
```
curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh
```
Mein eigenes Theme habe ich auch auf Githiub liegen. Einfach die denial.zsh-theme in den entsprechenden Ordner kopieren.
```
git clone https://github.com/dnlkng/oh-my-zsh.git
cp dev/oh-my-zsh/themes/denial.zsh-theme ~/.oh-my-zsh/themes
vim .zshrc
```
Und in der `~/.zshrc` folgende Zeile ersetzen:
```
ZSH_THEME="denial"
```
Wobei ich mittlerweile Powerlevel9k einsetze und damit sehr zufrieden bin.

### Nützliche oh my zsh plugins
#### Z
Damit kann man in die am häufigsten besuchten Ordner wechseln.

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
Für git sollten die wichtigsten Parameter gesetzt werden.
```
git config --global user.email "daniel@koenig.io"
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
Manchmal sind man pages einfach zu viel, um schnell ein einfachen Task zu erledigen. [Remember tar](https://xkcd.com/1168/)? Dafür gibt es tldr, eine community driven Sammlung von kurzen, knackigen Beschreibungen zu den wichtigsten commandline tools.
```
brew install tldr
```
Benutzung:
```
# tldr [commandname]
tldr tmux
```

## The Fuck
Es passiert immer mal wieder, man hackt ein Command in die Shell: Boom, Zack, Return... Und man hat sich vertippt. Wenn es nicht all zu weit vom original Command war, gibt man nun einfach nur `fuck` als nächsten Command ein und dieses Programm führt dann den eigentlichen Befehl aus.
<https://github.com/nvbn/thefuck>

```
brew install thefuck
```

 
## Sublime Text 3
```
ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl
```

## iTerm2
### Solarized Dark Theme

## Dotfiles
<https://dotfiles.github.io>

# Evaluate
<https://github.com/bhilburn/powerlevel9k>
<https://github.com/donnemartin/haxor-news#installation>
<https://taskwarrior.org/>
<https://github.com/Netflix-Skunkworks/go-jira>

# Resources
<http://sourabhbajaj.com/mac-setup/>
<https://terminalsare.sexy/>
<https://vimawesome.com>

