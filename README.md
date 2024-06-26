#### Instalar pacotes a seguir
```
sudo dnf install git curl build-essential dkms perl wget -y
sudo dnf install gcc make default-libmysqlclient-dev libssl-dev -y
sudo dnf install -y zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev llvm \
  libncurses5-dev libncursesw5-dev \
  xz-utils tk-dev libffi-dev liblzma-dev python3-openssl git
```

#### Instalar e configurar ZSH
```
sudo dnf install zsh -y
chsh -s /bin/zsh
zsh
```

#### Instalar Oh-my-zsh! (https://ohmyz.sh/)
```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

#### Instalar Spaceship Prompt (https://github.com/spaceship-prompt/spaceship-prompt)

```
git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1
ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"

Mudar: nano ~/.zshrc -> ZSH_THEME="spaceship"
```

#### Instalar Zsh Autosuggestions (https://github.com/zsh-users/zsh-autosuggestions)

```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

Mudar plugin:
nano ~/zshrc plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
```

#### Instalar Zsh Syntax Highlighting (https://github.com/zsh-users/zsh-syntax-highlighting)
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

#### Font optional (https://github.com/pdf/ubuntu-mono-powerline-ttf)
```
mkdir -p ~/.fonts
git clone https://github.com/pdf/ubuntu-mono-powerline-ttf.git ~/.fonts/ubuntu-mono-powerline-ttf
fc-cache -vf
```
#### Pyenv
```
pip install pyenv
```
# REBOOT!!!!!!!!!!!!!!!!!!!!!
