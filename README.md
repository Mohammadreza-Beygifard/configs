# configs
This repo will contain my configurations of tmux, fish, oh-my-zsh and nvim


## Before cloning this repo

### Step 1

Get sure that on .bashrc you include the `exports` related to the environment variables.

put these setting in your config file under .ssh if you use proxy
Host=github.com
User git
ProxyCommand=socat - PROXY:\<YOUR-PROXY-IP\>:%h:%p,proxyport= \<YOUR-PROXY-PORT\>

## After cloning this repo perform

```bash
git submodule init
```
```bash
git submodule update
```

## If you like ZSH jump to [ZSH-procedure](#zsh-procedure)

### Step2

Install fish from their [website](https://fishshell.com/)

### Step 3 

Install powerline fonts
```bash
sudo apt-get install fonts-powerline
```

### Step 4

Install Oh my Fish from their [website](https://github.com/oh-my-fish/oh-my-fish)

to choose a theme, like **agnoster**

```bash
omf install agnoster && omf theme agnoster
```

### Step 5

Install [jethrokuan/fzf](https://github.com/jethrokuan/fzf)

### Step6

Install tmux
```bash
sudo apt install tmux
```

Create a sLink with .thux.conf and tmux-packtheme, be careful that the name of the .tmux-themepack in home directory should be .tmux-themepack

```bash
ln -s ~/overall_configs/tmux-themepack ~/.tmux-themepack
```

```bash
ln -s ~/overall_configs/.tmux.conf ~/.tmux.conf
```
### Step7

Install SilverSercher-ag

```bash
sudo apt-get install silversearcher-ag
```
### Step8

```bash
sudo apt install npm
npm cache clean -f
```
If you have a problem with npm install and you are using a proxy check [solve npm problem with proxy](https://stackoverflow.com/questions/7559648/is-there-a-way-to-make-npm-install-the-command-to-work-behind-proxy)

### Step 9 

Install Bazel (If you need a build tool, [bazel](https://bazel.build/) is cool!)

```bash
npm install -g @bazel/bazelisk
```

---

## ZSH Procedure

Old procedure if you like to use ZSH

### Step2

Install zsh
```bash
sudo apt-get update
sudo apt-get install zsh
zsh --version
whereis zsh
```

```bash
ln -s ~/overall_configs/.zshrc ~/.zshrc
```
### Step3

Initialize oh-my-zsh

```bash
git submodule init ohmyzsh
```

```bash
git submodule update
```

and also install the theme you are currentlu using

in my case:
```bash
git clone https://github.com/sobolevn/sobole-zsh-theme.git ln -s $PWD/sobole-zsh-theme/sobole.zsh-theme ~/.oh-my-zsh/custom/themes/sobole.zsh-theme
```

### Step4

Install nodejs as almoste moste of nvim plugins need that.

```bash
sudo apt install npm
npm cache clean -f
sudo npm install -g n
sudo n stable
```

If you have a problem with npm install and you are using a proxy check [solve npm problem with proxy](https://stackoverflow.com/questions/7559648/is-there-a-way-to-make-npm-install-the-command-to-work-behind-proxy)

### Step5

Install tmux
```bash
sudo apt install tmux
```

Create a sLink with .thux.conf and tmux-packtheme, be careful that the name of the .tmux-themepack in home directory should be .tmux-themepack

```bash
ln -s ~/overall_configs/tmux-themepack ~/.tmux-themepack
```

```bash
ln -s ~/overall_configs/.tmux.conf ~/.tmux.conf
```
### Step6

Install SilverSercher-ag

```bash
sudo apt-get install silversearcher-ag
```

### Step7

Install neovim

```bash
sudo apt install neovim
```


```bash
ln -s ~/overall_configs/.config/nvim ~/.config/
```
