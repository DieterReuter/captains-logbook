
# Installation log book "Dieter's MacBook Pro"

![Mac](/images/logbook-MacBookPro3.png)


## 2017-11-06

* install `1Password` from AppStore
* install `Twitter` from AppStore
* keep `Twitter.app` in Dock
* install `Slack` from AppStore
* keep `Slack.app` in Dock
* install `Xcode 6.1.1` from AppStore
```bash
sudo xcodebuild -license
```

* install `iterm2` from https://www.iterm2.com
* remove `Terminal.app` from Dock
* keep `iterm2.app` in Dock

* restore ssh keys
```bash
mkdir -p ~/.ssh
```

* install .bash_prompt
```bash
cd ~
curl -O https://github.com/hypriot/os-rootfs/raw/master/builder/files/etc/skel/.bash_prompt
```
* create .profile
```bash
cat ~/.profile

# use color ls
export CLICOLOR=1
export LSCOLORS="ExGxBxDxCxEgEdxbxgxcxd"

if [ "$BASH" ]; then
  if [ -f ~/.bashrc ]; then
    . ~/.bashrc
  fi
fi

if [ -f ~/.bash_prompt ]; then
  . ~/.bash_prompt
fi
```

* install `homebrew`, see http://brew.sh
```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew doctor
brew update
brew install wget
brew install cask
```

* customize menu bar
  - attach `volume`
  - show `battery percentage`
  - show fast user switching menu as `Full Name`

* customize Accessibility/Zoom
  - Use scroll gesture with modifier keys to zoom to `^ Control`


DR, 2017
