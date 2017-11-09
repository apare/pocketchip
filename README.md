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
6. Install kbd zsh emacs git:
`sudo apt-get install kbd zsh emacs git`
7. Select utf8
8. Reduce font size:
`sudo dpkg-reconfigure console-setup`
9. get this repo:
`git clone https://github.com/apare/pocketchip.git`
10. install oh-my-zsh
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
11. Install spacemacs
`git clone https://github.com/syl20bnr/spacemacs ~/.emacs.d`
12. add keymap to zshrc
echo "source ~/pocketchip/keymap.sh" >> ~/.zshrc
13. generate a new ssh key
`ssh-keygen -t rsa -b 4096 -C "alex.pare.inc@gmail.com"`
14. show the public ssh key (you need to add it to github)
`cat .ssh/id_rsa.pub`
