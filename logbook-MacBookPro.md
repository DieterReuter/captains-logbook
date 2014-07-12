
# Installation log book "Dieter's MacBook Pro"

![Mac](/images/Screen\ Shot\ 2014-07-12\ at\ 13.00.44.png)


## 2014-07-09

* install `homebrew` [see](http://stackoverflow.com/questions/17271319/installing-pip-on-mac-os-x)
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

* install [grip](https://github.com/joeyespo/grip)
```bash
pip install grip
```

* install `Node` from [http://nodejs.org](http://nodejs.org) `node-v0.10.29.pkg`
* install `Sublime Text 3` from [http://www.sublimetext.com](http://www.sublimetext.com) `Sublime Text Build 3059.dmg`


## 2014-07-10

* install `Google Chrome` from [http://www.google.de/intl/us/chrome/browser/](http://www.google.de/intl/us/chrome/browser/) `googlechrome.dmg`
* install `Sqwiggle 0.5.2` from [https://www.sqwiggle.com](https://www.sqwiggle.com) `sqwiggle-0.5.2.dmg`

* install `GitHub for Mac` from [https://mac.github.com](https://mac.github.com) 
## 2014-07-11
* `brew install tree`


## 2014-07-12

* install `Twitter 3.0.1` from AppStore
* install `Microsoft Remote Desktop 8.0.7` from AppStore
* `brew install htop`


DR, 2014