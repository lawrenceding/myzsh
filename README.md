#my zsh configuration used in linux - ubuntu 13.10
## Install
### Linux
####1. install zsh
```
sudo apt-get install zsh
```
####2. install oh-my-zsh
```
git clone https://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh
```
####3. install my configuration
```
git clone https://github.com/lawrenceding/myzsh.git ~/.myzsh
```
####4. make the zsh as default shell
```
chsh -s /bin/zsh
```
After this, a re-login may be needed to make it work
####4. create links for zshrc and theme
```
ln -snf ~/.myzsh/zshrc ~/.zshrc
ln -snf ~/.myzsh/lawrence.zsh-theme ~/.oh-my-zsh/themes/lawrence.zsh-theme
```
