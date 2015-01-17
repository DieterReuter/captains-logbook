
# Installation log book "Dieter's MacBook Pro"

![Mac](/images/Screen Shot 2015-01-17 at 16.25.24.png)


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


DR, 2015
