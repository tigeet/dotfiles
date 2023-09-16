# Dotfiles

## Terminal

### iterm

        brew install iterm2 --cask

### zsh

        $ brew install zsh
        $ chsh -s /opt/homebrew/bin/zsh

### oh-my-zsh

        sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

### nerd font

        brew tap homebrew/cask-fonts
        brew install --cask font-hack-nerd-font

### p10k

        git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k

Set `ZSH_THEME="powerlevel10k/powerlevel10k"` in `~/.zshrc`

Comment out `  # typeset -g POWERLEVEL9K_CONTEXT_{DEFAULT,SUDO}_CONTENT_EXPANSION=` in `~/.p10k.zsh` to show `user@host`

### zsh plugins

#### zsh-autosuggestions

        git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

#### zsh-syntax-highlighting

        git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

Add `plugins=(git zsh-autosuggestions zsh-syntax-highlighting)` in `~/.zshrc`
