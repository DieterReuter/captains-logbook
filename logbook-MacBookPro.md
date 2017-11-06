
# Installation log book "Dieter's MacBook Pro"

![Mac](/images/logbook-MacBookPro.png)


## 2014-07-09

* install `homebrew`, see http://stackoverflow.com/questions/17271319/installing-pip-on-mac-os-x
```bash
ruby -e "$(curl -fsSL https://raw.github.com/mxcl/homebrew/go/install)"
```

* install `python` and `pip`
```bash
brew install python
```

* install `Xcode 5.1.1` from AppStore
```bash
sudo xcodebuild -license
brew doctor
```

```bash
Consider setting your PATH so that /usr/local/bin
occurs before /usr/bin. Here is a one-liner:
    echo export PATH='/usr/local/bin:$PATH' >> ~/.bash_profile
```
* correct the path issue reported by `brew doctor`
```bash
echo export PATH='/usr/local/bin:$PATH' >> ~/.bash_profile
```

* install `grip`, see https://github.com/joeyespo/grip
```bash
pip install grip
```

* install `Node.js` from http://nodejs.org `node-v0.10.29.pkg`
* install `Sublime Text 3` from http://www.sublimetext.com `Sublime Text Build 3059.dmg`


## 2014-07-10

* install `Google Chrome` from http://www.google.de/intl/us/chrome/browser `googlechrome.dmg`
* install `Sqwiggle 0.5.2` from https://www.sqwiggle.com `sqwiggle-0.5.2.dmg`
* install `GitHub for Mac` from https://mac.github.com


## 2014-07-11
* `brew install tree`
* install `nvm`, see https://github.com/creationix/nvm
```bash
curl https://raw.githubusercontent.com/creationix/nvm/v0.10.0/install.sh | bash
```
* `nvm install 0.10` install Node v0.10.x 
* `nvm ls`
* `nvm use current`


## 2014-07-12

* install `Twitter 3.0.1` from AppStore
* install `Microsoft Remote Desktop 8.0.7` from AppStore
* `brew install htop`
* install `ghost`, see http://docs.ghost.org/installation/mac or https://github.com/TryGhost/Ghost
```bash
mkdir -p ~/code/ghost
cd ~/code/ghost
curl -OL https://ghost.org/zip/ghost-0.4.2.zip
unzip ghost-0.4.2.zip
npm install --production
npm start
```
* `open http://127.0.0.1:2368` to open your local blog in your favorite browser
* `open http://127.0.0.1:2368/ghost` to create an Admin account
* install `buster`, see https://github.com/axitkhurana/buster
* `pip install buster`
* `pip install wget`


## 2014-07-13

* install `VirtualBox 4.3.12` from https://www.virtualbox.org/wiki/Downloads
* install `VirtualBox 4.3.12 Oracle VM VirtualBox Extension Pack`
* install `Vagrant 1.6.3` from http://www.vagrantup.com/downloads.html
* install Vagrant PlugIns
```bash
vagrant plugin install vagrant-cachier
vagrant plugin install vagrant-pristine
vagrant plugin install vagrant-vbox-snapshot
```
* list all installed Vagrant PlugIns
```bash
vagrant plugin list
vagrant-cachier (0.7.2)
vagrant-login (1.0.1, system)
vagrant-pristine (0.3.0)
vagrant-share (1.1.0, system)
vagrant-vbox-snapshot (0.0.5)
```
* `brew install wakeonlan`
```bash
# wake up my NUC device on 192.168.178.143
wakeonlan c0:3f:d5:63:1e:94
```
* `brew install macvim`
* `brew install vim --override-system-vi`
* customizing `Sublime Text 3`, see http://www.sublimetext.com/docs/3/osx_command_line.html
```bash
ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl
```
* install `iTerm 2`, see http://www.iterm2.com
* install some Node modules
```bash
nvm use 0.10.26
npm install -g jsontool
npm install -g js-beautify
npm install -g http-console
```
* install `Kindle 1.10.6` from AppStore


## 2014-07-18
* install `Wallpaper by Behance 1.0.13` from AppStore
* install `Work in Progress 1.2.5` from AppStore
* install `Keynote 6.2` from AppStore


## 2014-07-20
* install `VMware OVF Tool` directly from VMware, see https://my.vmware.com/de/group/vmware/details?downloadGroup=OVFTOOL350&productId=352 (note: you'll need a VMware account)
```bash
download VMware-ovftool-3.5.0-1274719-mac.x64.dmg
hdiutil attach VMware-ovftool-3.5.0-1274719-mac.x64.dmg
cd /Volumes/VMware-ovftool-3.5.0-1274719-mac.x64.dmg
sudo installer -verbose -pkg VMware\ OVF\ Tool.pkg -target /
hdiutil info
hdiutil detach /dev/disk1s2
ln -s /Applications/VMware\ OVF\ Tool/ovftool /usr/local/bin/ovftool
```


## 2014-07-21
* `brew install httpie`
* `sudo pip install pyvmomi`, see http://www.virtuallyghetto.com/2013/12/early-xmas-gift-from-vmware-pyvmomi.html
* `sudo gem install rbvmomi`
* `sudo gem install nokogiri --version "=1.5.5"`, to solve version conflicts with rbvmomi


## 2014-07-22
* install `Wireshark 1.10.8`, see http://www.wireshark.org/download.html
* install `XQuartz 2.7.6`, see http://xquartz.macosforge.org/landing/


## 2014-07-23
* install `Silverlight.dmg` just to watch a Webinar
* `brew install tcpflow`, details see https://developer.apple.com/library/ios/qa/qa1176/_index.html#//apple_ref/doc/uid/DTS10001707-CH1-SECGETTINGSTARTEDWITHTCPFLOW


## 2014-07-26
* install `Wunderlist 2.3.5` from AppStore
* install Vagrant plug-in `vagrant-serverspec`
```bash
vagrant plugin install vagrant-serverspec
```
* install `packer 0.6.0` as decribed in http://www.packer.io/intro/getting-started/setup.html
```bash
brew tap homebrew/binary
brew install packer
```
* install `VirtualBox 4.3.14` from https://www.virtualbox.org/wiki/Downloads
* install `VirtualBox 4.3.14 Oracle VM VirtualBox Extension Pack`
* install `VMware Fusion 6.0.4 Trial` from https://www.vmware.com/go/tryfusion
* changed vagrant snapshot plugin to support more providers
```bash
vagrant plugin uninstall vagrant-vbox-snapshot
vagrant plugin install vagrant-multiprovider-snap
```


* fixing problems with `nokogiri` for Homebrew 0.9.5, see http://nokogiri.org/tutorials/installing_nokogiri.html
```bash
brew link libxml2 libxslt
brew link libxml2 libxslt --force
```
```bash
mkdir libiconv
cd libiconv
wget http://ftp.gnu.org/pub/gnu/libiconv/libiconv-1.13.1.tar.gz
tar xvfz libiconv-1.13.1.tar.gz
cd libiconv-1.13.1
./configure --prefix=/usr/local/Cellar/libiconv/1.13.1
make
sudo make install
```
```bash
sudo gem install nokogiri -- --with-xml2-include=/usr/local/Cellar/libxml2/2.7.8/include/libxml2 \
                        --with-xml2-lib=/usr/local/Cellar/libxml2/2.7.8/lib \ 
                        --with-xslt-dir=/usr/local/Cellar/libxslt/1.1.26 \
                        --with-iconv-include=/usr/local/Cellar/libiconv/1.13.1/include \
                        --with-iconv-lib=/usr/local/Cellar/libiconv/1.13.1/lib
```

* repair Vagrant installation
```bash
mv ~/.vagrant.d ~/.vagrant.d-sav
mv ~/.vagrant.d-sav/boxes ~/.vagrant.d/
vagrant plugin install vagrant-cachier
vagrant plugin install vagrant-pristine
vagrant plugin install vagrant-serverspec
vagrant plugin install vagrant-multiprovider-snap
```

Next try, see http://stackoverflow.com/questions/19569031/error-failed-to-build-gem-native-extension-on-mavericks
```bash
xcode-select --install
sudo gem install nokogiri
```
OK, that worked fine!


## 2014-07-27
* buying a license for the `Vagrant VMware Fusion provider`, see http://www.vagrantup.com/vmware#buy-now
* install `Vagrant VMware Fusion provider`
```bash
vagrant plugin install vagrant-vmware-fusion
vagrant plugin license vagrant-vmware-fusion license.lic
```
```bash
vagrant plugin list
vagrant-cachier (0.8.0)
vagrant-login (1.0.1, system)
vagrant-multiprovider-snap (0.0.11)
vagrant-pristine (0.3.0)
vagrant-serverspec (0.1.0)
vagrant-share (1.1.0, system)
vagrant-vmware-fusion (2.4.1)
```
* install `Dropbox 2.10.3` from https://www.dropbox.com/
* install `Suspicious Package 1.3` from http://www.mothersruin.com/software/SuspiciousPackage/


## 2014-07-28
* `brew install cdrtools`


## 2014-08-06 
* install `Atom` from https://atom.io


## 2014-08-08 
* `sudo gem install bundle`
* `sudo gem install dashing`


## 2014-08-12 
* instal GO 1.3 from http://golang.org/dl/go1.3.darwin-amd64-osx10.8.pkg


## 2014-08-17
* install `Skala Color` color picker from http://bjango.com/mac/skalacolor/
* install `Colors` color picker from http://mattpatenaude.com, details found here http://osxdaily.com/2011/09/12/digital-color-meter-picker-replacement-for-mac-os-x-lion/
* `brew search imagemagick`
* install Chrome ColorZilla, see http://www.colorzilla.com/chrome/


## 2014-08-22
* use `Oracle SQL Developer` to connect to a MS SQL Azure Server, see http://stuffthatspins.com/2014/04/07/connect-to-mssql-server-client-mac-os-x-sqlserver-client-mavericks/
* install `Oracle SQL Developer 4.0.2 (4.0.2.15.21)` from http://www.oracle.com/technetwork/developer-tools/sql-developer/overview/index-097090.html
* install `Java for Mac OS X 10.5, Update 1` from http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html
* install `jTDS - SQL Server and Sybase JDBC driver` from http://sourceforge.net/projects/jtds/files/
* install `MySQL Connector/J JDBC driver` from http://dev.mysql.com/downloads/connector/j/5.0.html


## 2014-08-23
* install driver for `Wacom Bamboo Pen and Touch, CTH-461` 
*    (Driver 5.3.3-3 for OS X 10.8, 10.7 & 10.6, 9 Sep 2013, from http://us.wacom.com/en/support/legacy-drivers/)
*    MacOSX - Driver 5.3.5-4 (10.7x - 10.9x), 08/20/2014, 29 MB, from http://us.wacom.com/en/support/drivers/


## 2014-08-31
* install GOLANG DevEnv, see http://railskey.wordpress.com/2014/05/31/install-gogolang-on-ubuntu/
* install `gvm` from https://github.com/moovweb/gvm
```bash
brew install mercurial
bash < <(curl -s -S -L https://raw.githubusercontent.com/moovweb/gvm/master/binscripts/gvm-installer)
gvm install go1.3.1
gvm use go1.3.1 --default
gvm list
```


## 2014-09-05
* install Atom plugin `go-plus` from https://atom.io/packages/go-plus
* `apm install go-plus`


## 2014-09-05
* install `OSXFUSE 2.7.0` and `SSHFS 2.5.0` from http://osxfuse.github.io


## 2014-09-07
* install `boot2docker` from https://github.com/boot2docker/osx-installer/releases


## 2014-09-09
* install `GoConvey` from http://goconvey.coreleases
* `go get github.com/smartystreets/goconvey`
* install `Sublime Text 2` from http://www.sublimetext.com `Sublime Text 2.0.2.dmg`
* install `Sublime Package Control`from https://sublime.wbond.net/installation#st2
* install `gosublime` from https://github.com/DisposaBoy/GoSublime


## 2014-09-27
* `brew install xz`


## 2014-10-02
* install `Vagrant 1.6.5` from http://www.vagrantup.com/downloads.html
* install `VirtualBox 4.3.16` from https://www.virtualbox.org/wiki/Downloads
* install `VirtualBox 4.3.16 Oracle VM VirtualBox Extension Pack`
* install `Panamax` from http://panamax.io/get-panamax/
* `brew install http://download.panamax.io/installer/brew/panamax.rb`


## 2014-10-03
* `brew install jq`


## 2014-10-31
* `brew upgrade packer` to v0.7.2


## 2014-12-13
* `brew upgrade packer` to v0.7.5
* install `Vagrant 1.7.1` from http://www.vagrantup.com/downloads.html
* install `VirtualBox 4.3.20` from https://www.virtualbox.org/wiki/Downloads
* install `VirtualBox 4.3.20 Oracle VM VirtualBox Extension Pack`


## 2015-01-15
* `pip install virtualenv`
```bash
brew install autoenv
echo 'source /usr/local/opt/autoenv/activate.sh' >> ~/.bash_profile
```
* `brew install ansible`
* install `SizeUp` from http://www.irradiatedsoftware.com/sizeup/


## 2015-01-16
* install `Microsoft OneNote` from AppStore https://itunes.apple.com/de/app/microsoft-onenote/id784801555?mt=12 
* install `Evernote` from AppStore https://itunes.apple.com/de/app/evernote/id406056744?mt=12
* install `BitTorrent Sync` from http://www.getsync.com


DR, 2015
