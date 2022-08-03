# Linux-Ubuntu

# Executar comandos a seguir para atualizar os pacotes
sudo apt update -y
sudo apt upgrade -y

# Instalar pacotes a seguir
sudo apt install dkms make perl gcc build-essential git curl -y

# Baixar e instalar VS Code: https://code.visualstudio.com/download
# Baixar e instalar Google Chrome: https://www.google.com/intl/pt-BR/chrome/

# Instalar Python 3.10 (opcional)
sudo apt install python3.10-full python3.10-dev

# Instalar e configurar ZSH
sudo apt install zsh -y
chsh -s /bin/zsh
zsh

# Instalar Oh-my-zsh! -> https://ohmyz.sh/
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# Instalar Zsh Syntax Highlighting
# https://github.com/zsh-users/zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

# Instalar Spaceship Prompt
# https://github.com/spaceship-prompt/spaceship-prompt
git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1
ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"

# Instalar Zsh Autosuggestions
# https://github.com/zsh-users/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

# Mudar ~/.zshrc -> ZSH_THEME="spaceship"

# Mudar plugins
# plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

# Font optional (https://github.com/pdf/ubuntu-mono-powerline-ttf)
mkdir -p ~/.fonts
git clone https://github.com/pdf/ubuntu-mono-powerline-ttf.git ~/.fonts/ubuntu-mono-powerline-ttf
fc-cache -vf

# REBOOT

sudo apt install gnome-tweaks gnome-shell-extensions -y

gnome shell integration: https://chrome.google.com/webstore/detail/gnome-shell-integration/gphhapmejobijbbhgpjhcjognlahblep

gnome shell extensions:  https://extensions.gnome.org/

Lista de extensões usadas:

- User theme
- ArcMenu
- Blur my Shell
- Dash to Dock(depende da versão do gnome)
- Extension List
- Screenshot Tool
- OpenWeather
- Sound Input & Output Device Chooser
- Tiling Assistant
- Vitals

sudo apt install git

git clone https://github.com/vinceliuice/WhiteSur-gtk-theme.git

cd WhiteSur-gtk-theme

./install.sh -t all -N glassy -s 220 -i ubuntu

sudo ./tweaks.sh -g

WhiteSur icon theme: https://www.pling.com/p/1405756/
McMojave cursors: https://www.pling.com/p/1355701/
WhiteSur Wallpaper: https://github.com/vinceliuice/WhiteSur-wallpapers

criar a pasta .icons no /home e extrair o icon theme e o cursor nela
