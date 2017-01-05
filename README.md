
# z.complete.me
## 'cwd' for all open zsh sessions

## What it does:

This plugin allows to complete the 'cwd' of other Zsh sessions. Sounds
complicated but is rather simple. E.g. if you have three zsh sessions open, in
each session you are in a different folder, you can hit Ctrl+v in one session
to show you the current working directory of the other open zsh sessions.

## How it works:

* Depending on the system it uses a combination of pidof, lsof, pgrep and procfs to determine all zsh PIDs and its working directories
* Everything is fed into zsh's completion magic

## Installation:

* Install [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
* Then
```
cd ~/.oh-my-zsh/plugins
git clone https://github.com/deathjest3r/z.complete.me.git
vim ~/.zshrc
```

Add z.complete.me to plugins entry to ```~./.zshrc```
```
plugins=(... z.complete.me)
```
* Done
