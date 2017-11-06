
# Installation log book "Dieter's MacBook Pro"

![Mac](/images/logbook-MacBookPro3.png)


## 2017-11-06

* install `1Password` from AppStore
* install `SizeUp` from http://www.irradiatedsoftware.com/sizeup/
* install `Bear` from AppStore
* install `Microsoft OneNote` from AppStore
* install `Twitter` from AppStore
* keep `Twitter.app` in Dock
* install `Slack` from AppStore
* keep `Slack.app` in Dock
* install `Xcode 6.1.1` from AppStore
```bash
sudo xcodebuild -license
```

* configure git user
```
git config --global user.email "dieter.reuter@me.com"
git config --global user.name "Dieter Reuter"
```

* restore ssh keys
```bash
mkdir -p ~/.ssh
```

* install .bash_prompt
```bash
cd ~
curl -O https://github.com/hypriot/os-rootfs/raw/master/builder/files/etc/skel/.bash_prompt
```
* create .bash_profile
```bash
cat ~/.bash_profile

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

# see: https://gist.github.com/mischah/8149239
# Move next only if `homebrew` is installed
if command -v brew >/dev/null 2>&1; then
  # Load rupa's z if installed
  [ -f $(brew --prefix)/etc/profile.d/z.sh ] && source $(brew --prefix)/etc/profile.d/z.sh
fi
```
```
brew install z
```

* install `homebrew`, see http://brew.sh
```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew doctor
brew update
brew install cask
```
```bash
brew install wget
brew install hub
brew install jq
brew install xz
brew install tree
brew install p7zip
brew install pv
brew cask install iterm2
```

* remove `Terminal.app` from Dock
* keep `iterm2.app` in Dock

* customize menu bar
  - attach `volume`
  - show `battery percentage`
  - show fast user switching menu as `Full Name`

* customize Accessibility/Zoom
  - Use scroll gesture with modifier keys to zoom to `^ Control`

* set power mode to never sleep
```bash
sudo pmset -a sleep 0
```

* install Sublime Text 3
```bash
brew cask install sublime-text
```

* install `VirtualBox-5.2.0-118431-OSX.dmg` from https://www.virtualbox.org/wiki/Downloads

* install Vagrant 2.0.1
```bash
brew cask install vagrant
brew install vagrant-completion
```


DR, 2017
