# Things
Workflow that I usually do when I need to set up another Laptop

## Macbook :computer:

### System Preferences
- [ ] Check if System Updates are present
### Users & Groups
- [ ] Login Options -> Change fast user switching menu as Icon
- [ ] Set up Password, Apple ID, Picture, etc.
### Trackpad
- [ ] Enable Tap to click with one finger
- [ ] In _More Gestures_  remove notification Center and Launchpad Flagd
### Dock
- [ ] Make the size of icons Small
### Finder
- [ ] Change the New finder window show to open in your Home Directory
### Sidebar
- [ ] Add Home and your Code Directory
- [ ] Uncheck all Shared boxes
### Menubar
- [ ] Remove Display and Spotlight icons
- [ ] Remove display day of the week
- [ ] Change battery to Show percentage symbols

### Accounts
- [ ] Add an iCloud account and sync Calendar, Find my Mac, Contacts, etc.


## Bootstrap minimal DEV requirements :beers:

### XCODE & HomeBrew

- [ ] Install XCODE _(dont' forget to install the Devices Emulators)_
```
xcode-select --install
```
- [ ] Install Brew
```
//install script
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"

//Set brew path
echo 'PATH="/usr/local/bin:$PATH"' >> ~/.bash_profile

//Check if everything is good
brew doctor

```

### Shell
- [ ] Install Warp
```
brew install --cask warp
```
- [ ] Install oh-my-zsh with these [instructions](https://sourabhbajaj.com/mac-setup/iTerm/zsh.html).
- [ ] Install Tree
```
brew install tree

```
### Git and GitHub
- [ ] install Git with these  [instructions](https://sourabhbajaj.com/mac-setup/Git/).
### Node and package Manager
- [ ] Install Volta
```
# install Volta
curl https://get.volta.sh | bash

# install Node and package managers
volta install node && volta install npm && volta install yarn && volta install pnpm
```
- [ ] Install Devenv
```
# Install Nix
sh <(curl -L https://nixos.org/nix/install) --daemon

#Install Cachix
nix-env -iA cachix -f https://cachix.org/api/v1/install
cachix use devenv

#Install Devenv
nix-env -if https://github.com/cachix/devenv/tarball/latest
```


