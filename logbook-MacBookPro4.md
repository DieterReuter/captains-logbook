
# Installation log book "Dieter's MacBook Pro"

![Mac](/images/logbook-MacBookPro4.png)


## 2018-12-20

* clean install of macOS Mojave 10.14.2

* restore basic .dotfiles (from backup)
```
.bash_profile
.bash_prompt
.bashrc
.profile
```

* restore ssh keys
```bash
mkdir -p ~/.ssh
```

* configure git user
```
git config --global user.email "dieter.reuter@me.com"
git config --global user.name "Dieter Reuter"
```

* install `1Password7` from AppStore
* install `Xcode 9.1` from AppStore
```bash
sudo xcodebuild -license
```

* install `homebrew`, see http://brew.sh
```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew doctor
brew update
brew install cask
```

```bash
brew install z
brew install wget
brew install hub
brew install jq
brew install xz
brew install tree
brew install p7zip
brew install pv
brew cask install iterm2
```

* install Sublime Text 3
```bash
brew cask install sublime-text
```

* remove `Terminal.app` from Dock
* keep `iterm2.app` in Dock

* install `Microsoft OneNote` from AppStore
* install `Microsoft Remote Desktop 10` from AppStore
* install `Slack` from AppStore
* install `SizeUp` from http://www.irradiatedsoftware.com/sizeup/

* customize menu bar
  - attach `volume`
  - show `battery percentage`
  - show fast user switching menu as `Full Name`

* customize Accessibility/Zoom
  - Use scroll gesture with modifier keys to zoom to `^ Control`

* customize secure screen lock
  - Require password `immediately` after sleep or screen saver begins

* set power mode to never sleep
```bash
sudo pmset -a sleep 0
```

* install shellcheck tool
```bash
brew install shellcheck
```

* install Visual Studio Code
```bash
brew cask install visual-studio-code
```


---


## More installs for later


* install `VirtualBox-5.2.0-118431-OSX.dmg` from https://www.virtualbox.org/wiki/Downloads

* install Vagrant 2.0.1
```bash
brew cask install vagrant
brew install vagrant-completion
```


* install `Plantronics Hub (Desktop)` from http://www.plantronics.com/us/category/software/


* install MiniShift
```bash
brew cask install minishift
```


* Install driver for USB2Serial from http://www.prolific.com.tw/us/showproduct.aspx?p_id=229&pcid=41
  File=PL2303_MacOSX_1.6.1_20170620.zip


* install OSX driver for `Digitus DN-3023` USB3.0-Ethernet Adapter from http://www.digitus.info/en/products/network/gigabit-ethernet-network/network-interface-cards/r-gigabit-ethernet-usb-30-adapter-dn-3023/
* download `AX88179_178A.dmg` from http://ftp.assmann.com/pub/DN-/DN-3023___4016032318385/DN-3023_driver_Driver%20MAC10.6-10.12_20161024.zip


* Install Terraform
```bash
brew install terraform

terraform version
Terraform v0.11.1
```


DR, 2018
