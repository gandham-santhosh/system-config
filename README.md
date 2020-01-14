# system-config
1. Install pre-requisites
sudo apt install git-core zsh
2. Install Oh-My-Zsh from Robby Russell’s repository
  $ sh -c “$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
3. Install the powerline fonts
sudo apt install fonts-powerline	
4. vim ~/.zshrc and update plugins array 
plugins=(
    git
    colored-man-pages
    vi-mode
    history
    history-substring-search
    z
    zsh-autosuggestions
    forgit
    zsh-syntax-highlighting
    )
5. Install the plugins
   git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
   git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
6. Change theme by updating ZSH_THEME="agnoster"
7. Install fzf fuzzy finder plugin
   https://github.com/junegunn/fzf

