# MyDebianConfig
💻 -h3x0v3rl0rd-


### Terminal Config
```
sudo apt install terminator tmux fish
chsh -s `which fish` (make fish default shell)
set fish_greeting ( remove fish greeting)
```
### Tmux Config
```
git clone https://github.com/h3x0v3rl0rd/.tmux.git
ln -s -f .tmux/.tmux.conf
cp .tmux/.tmux.conf.local .
### close and reopen tmux
```
### change tmux default shell
```
nano .tmux.conf

# set shell
set -g default-shell /bin/fish
```
### VSCodium
```
wget -qO - https://gitlab.com/paulcarroty/vscodium-deb-rpm-repo/-/raw/master/pub.gpg | gpg --dearmor | sudo dd of=/etc/apt/trusted.gpg.d/vscodium.gpg

echo 'deb https://paulcarroty.gitlab.io/vscodium-deb-rpm-repo/debs/ vscodium main' | sudo tee --append /etc/apt/sources.list.d/vscodium.list

sudo apt update && sudo apt install codium
sudo apt install python3 python3-pip -y
```
