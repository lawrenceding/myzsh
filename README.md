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

ln -snf ~/.myzsh/zshrc ~/.zshrc
ln -snf ~/.myzsh/lawrence.zsh-theme ~/.oh-my-zsh/themes/lawrence.zsh-theme
```
####4.add fonts for prompt fancy
Got the powerline font from https://gist.github.com/qrush/1595572
and don't need to download manual, it's in the repository already.
```
mkdir ~/.fonts
cp ~/.myzsh/fonts-for-airline/Inconsolata-dz-Powerline.otf ~/.fonts
fc-cache -vf
```
####5. make the zsh as default shell
```
chsh -s /bin/zsh
```
After this, a re-login may be needed to make it work
