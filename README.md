# MyDebianConfig

### Terminal Config
```
sudo apt install terminator tmux fish
chsh -s `which fish` (make fish default shell)
set fish_greeting ( remove fish greeting)
```
### Tmux Config
```
git clone https://github.com/3hydraking/.tmux.git
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
