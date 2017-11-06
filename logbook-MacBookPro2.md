
# Installation log book "Dieter's MacBook Pro"

![Mac](/images/logbook-MacBookPro2.png)


## 2015-01-17

* install `1Password` from https://agilebits.com/onepassword
* install `SizeUp` from http://www.irradiatedsoftware.com/sizeup/
* install `Evernote` from AppStore
* install `Microsoft OneNote` from AppStore
* install `Microsoft Remote Desktop` from AppStore
* install `Slack` from AppStore
* install `Wunderlist` from AppStore
* install `Kindle` from AppStore
* install `Slack` from AppStore
* install `Twitter` from AppStore
* install `Xcode 6.1.1` from AppStore
```bash
sudo xcodebuild -license
```

* install `homebrew`, see http://brew.sh
```bash
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew doctor
brew update
brew install cask
```
* install cask, see http://caskroom.io
```bash
brew install caskroom/cask/brew-cask
```

* install `python` and `pip`
```bash
brew install python
pip install --upgrade setuptools
pip install --upgrade pip
```

* install `VirtualBox 4.3.20` from https://www.virtualbox.org/wiki/Downloads
* install `VirtualBox 4.3.20 Oracle VM VirtualBox Extension Pack`
* install `Packer 0.7.5` as decribed in http://www.packer.io/intro/getting-started/setup.html
```bash
brew tap homebrew/binary
brew install packer
brew install homebrew/completions/packer-completion
```
* install `Vagrant 1.7.2`
```bash
brew cask install vagrant
brew install vagrant-completion
```
* install vagrant plugins
```bash
#vagrant plugin install vagrant-cachier
vagrant plugin install vagrant-pristine
vagrant plugin install vagrant-serverspec
vagrant plugin install vagrant-multiprovider-snap
vagrant plugin install vagrant-triggers
```
```bash
vagrant plugin list
vagrant-multiprovider-snap (0.0.14)
vagrant-pristine (0.3.0)
vagrant-serverspec (0.1.0)
vagrant-share (1.1.3, system)
vagrant-triggers (0.5.0)
```

* `brew install jq`
* `brew install xz`
* `brew install tree`
* `brew install wakeonlan`
* `pip install virtualenv`
* install `autoenv`
```bash
brew install autoenv
echo 'source /usr/local/opt/autoenv/activate.sh' >> ~/.bash_profile
```
* `brew install ansible`
* `pip install grip` see https://github.com/joeyespo/grip
* `brew install --HEAD hub`
* `brew cask install iterm2`


## 2015-01-18

* set power mode to never sleep
`sudo pmset -a sleep 0`


## 2015-01-19
```bash
vagrant plugin install vagrant-reload
```
* install OSX driver for `Digitus DN-3023` USB3.0-Ethernet Adapter from http://www.digitus.info/en/products/network/gigabit-ethernet-network/network-interface-cards/r-gigabit-ethernet-usb-30-adapter-dn-3023/
* download `AX88179_178A.dmg` from http://ftp.assmann.com/pub/DN-/DN-3023___4016032318385/DN-3023_driver_driver%20Mac10.6-10.10_20140926.zip
* install `Adobe Flash`


## 2015-01-22
```bash
vagrant plugin install vagrant-hostmanager
```
```bash
vagrant plugin list
vagrant-hostmanager (1.5.0)
vagrant-multiprovider-snap (0.0.14)
vagrant-pristine (0.3.0)
vagrant-reload (0.0.1)
vagrant-serverspec (0.1.0)
vagrant-share (1.1.3, system)
vagrant-triggers (0.5.0)
```


## 2015-01-24
* Install driver for USB2Serial from http://www.prolific.com.tw/us/showproduct.aspx?p_id=229&pcid=41
  File=PL2303_MacOSX_v1.5.1.pkg


## 2015-01-29
* `brew install ssh-copy-id`
* `brew cask install atom`


## 2015-01-30
* `brew install p7zip`


## 2015-01-31
# ValueError: unknown locale: UTF-8
```
cat << EOF | "tee -a .bash_profile"
export LC_ALL=en_US.UTF-8
export LANG=en_US.UTF-8
EOF
```
`brew cask install alfred`


## 2015-02-09
`brew cask install macpass`


## 2015-02-10
`brew cask install xquartz`
`brew cask install wireshark`


## 2015-02-18
# permanently set hostname from cli
```
sudo scutil --set HostName DietersMBP
sudo scutil --set HostName DietersMacBookPro
```


## 2015-02-24
`brew install pigz`


## 2015-02-25
`brew cask install emacs`
`brew cask install macvim`
`brew install vim`
`brew install macvim`
`brew link --overwrite macvim`

* install RVM (see https://hpc.uni.lu/blog/2014/create-a-sandboxed-python-slash-ruby-environment/)
```
gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
curl -sSL https://get.rvm.io | bash -s stable
cat << EOF >> ~/.bash_profile
export PATH="$PATH:$HOME/.rvm/bin" # Add RVM to PATH for scripting
[[ -s "$HOME/.rvm/scripts/rvm" ]] && source "$HOME/.rvm/scripts/rvm" # Load RVM into a shell session *as a function*
EOF
source ~/.bash_profile
rvm install 2.0.0 --default
ruby -v
ruby 2.0.0p598 (2014-11-13 revision 48408) [x86_64-darwin14.1.0]
rvm @global do gem install bundler
```
`brew install pv`


## 2015-02-27
* install gvm and go
```
bash < <(curl -s -S -L https://raw.githubusercontent.com/moovweb/gvm/master/binscripts/gvm-installer)
gvm install go1.4.2
gvm use go1.4.2 --default
```


## 2015-02-28
`brew install hugo`
`pip install --upgrade pip`
`pip install Pygments --upgrade`


## 2015-03-06
* install nvm
```bash
brew install nvm
mkdir ~/.nvm
cat << EOF >> ~/.bash_profile
export NVM_DIR=~/.nvm
source $(brew --prefix nvm)/nvm.sh
EOF
source ~/.bash_profile
```
```bash
nvm install v0.12.0
nvm use 0.12
```


## 2015-03-12
`brew cask install sublime-text`
* install `Kitematic 0.5.11` from https://kitematic.com
* install `VirtualBox-4.3.24-98716-OSX.dmg` from https://www.virtualbox.org/wiki/Downloads
* install `VirtualBox-4.3.24-98716-OSX.dmg Oracle VM VirtualBox Extension Pack`


## 2015-03-26
`brew install socat`


## 2016-03-04
* install `VirtualBox-5.0.14-105127-OSX.dmg` from https://www.virtualbox.org/wiki/Downloads
* install `VirtualBox-5.0.14-105127-OSX.dmg Oracle VM VirtualBox Extension Pack`
```bash
vagrant plugin install vagrant-pristine
vagrant plugin install vagrant-reload
vagrant plugin install vagrant-hostmanager
vagrant plugin install vagrant-multiprovider-snap
vagrant plugin install vagrant-triggers
vagrant plugin install vagrant-share
vagrant plugin install vagrant-serverspec
vagrant plugin install vagrant-esxi
vagrant plugin install vagrant-digitalocean
vagrant plugin install vagrant-vmware-fusion
vagrant plugin license vagrant-vmware-fusion /Users/dieter/software-licenses/vagrant-vmware-fusion/license.lic
```
```bash
vagrant plugin list
vagrant-digitalocean (0.7.10)
vagrant-esxi (0.0.1)
vagrant-hostmanager (1.8.1)
vagrant-multiprovider-snap (0.0.14)
vagrant-pristine (0.3.0)
vagrant-reload (0.0.1)
vagrant-serverspec (1.1.0)
vagrant-share (1.1.5)
vagrant-triggers (0.5.2)
vagrant-vmware-fusion (4.0.8)
```

DR, 2016
