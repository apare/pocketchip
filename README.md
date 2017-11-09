1. Change password:
`passwd`
2. change hostname:
`sudo nmtui`
3. Connect to wifi:
`nmtui`
4. SSH the pocketchip from an other pc (because the colon is not accessible)
`ssh chip@192.168.1.xxx`
5. Update packages:
`sudo apt-get update`
6. Install kbd zsh emacs git vim locales:
`sudo apt-get install zsh emacs git vim locales`
7. Select utf8
`sudo dpkg-reconfigure locales`
select `en_US.UTF-8 UTF-8` then `en_US.UTF-8`
8. Add this to utf8 to zsh
```
export LC_ALL=en_US.UTF-8
export LANG=en_US.UTF-8
export LANGUAGE=en_US.UTF-8
```
9. Reduce font size:
`sudo dpkg-reconfigure console-setup`
10. get this repo:
`git clone https://github.com/apare/pocketchip.git`
11. install oh-my-zsh
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
12. Install spacemacs
`git clone https://github.com/syl20bnr/spacemacs ~/.emacs.d`
13. add keymap to zshrc
echo "source ~/pocketchip/keymap.sh" >> ~/.zshrc
14. generate a new ssh key
`ssh-keygen -t rsa -b 4096 -C "alex.pare.inc@gmail.com"`
15. show the public ssh key (you need to add it to github)
`cat .ssh/id_rsa.pub`
16.  Add `/usr/bin/loadkeys /home/chip/pocketchip/keymap.kmap` in `/etc/rc.local`
17. install nodejs
`curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -` then `sudo apt-get install nodejs build-essential`
