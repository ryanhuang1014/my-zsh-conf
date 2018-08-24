# my zsh configuration file
---

My configuration is composed of two parts: 1) install necessary softwares, 2) use the customized `.zshrc` file.

## install necessary softwares

sudo apt install zsh

sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

git clone https://github.com/oskarkrawczyk/honukai-iterm-zsh.git

cp honukai-iterm-zsh/honukai.zsh-theme ~/.oh-my-zsh/custom/themes/

sudo apt install autojump 

git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

## replace the default `.zshrc`

cp my-zsh-config/.zshrc ~/