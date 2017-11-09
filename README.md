### Change password:
`passwd`
### Connect to wifi:
`nmtui`
### SSH the pocketchip from an other pc (because the colon is not accessible)
`ssh chip@192.168.1.xxx`
### Update packages:
`sudo apt-get update`
### Install kbd zsh emacs git vim locales:
`sudo apt-get install zsh emacs git vim locales`
### set zsh as default
`chsh` then type `/bin/zsh`
### Select utf8
`sudo dpkg-reconfigure locales`
select `en_US.UTF-8 UTF-8` then `en_US.UTF-8`
### Add this to utf8 to zsh
```
export LC_ALL=en_US.UTF-8
export LANG=en_US.UTF-8
export LANGUAGE=en_US.UTF-8
```
### Reduce font size:
`sudo dpkg-reconfigure console-setup`
### get this repo:
`git clone https://github.com/apare/pocketchip.git`
### install oh-my-zsh
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
### Install spacemacs
`git clone https://github.com/syl20bnr/spacemacs ~/.emacs.d`
### add keymap to zshrc
add `source ~/pocketchip/keymap.sh` to `~/.zshrc`
### generate a new ssh key
`ssh-keygen -t rsa -b 4096 -C "alex.pare.inc@gmail.com"`
### show the public ssh key (you need to add it to github)
`cat .ssh/id_rsa.pub`
###  Setup keymap
Add `/usr/bin/loadkeys /home/chip/pocketchip/keymap.kmap` in `/etc/rc.local`
### install nodejs
`curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -` then `sudo apt-get install nodejs build-essential`
