# system-config
Steps to setup
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

Update git config to enable credential helper. Add the follwing lines in ~/.zshrc file
## GIT ###
GIT_AUTHOR_NAME="gandham-santhosh"
GIT_COMMITTER_NAME="$GIT_AUTHOR_NAME"
git config --global user.name "$GIT_AUTHOR_NAME"
GIT_AUTHOR_EMAIL="santhosh.g@optit.in"
GIT_COMMITTER_EMAIL="$GIT_AUTHOR_EMAIL"
git config --global user.email "$GIT_AUTHOR_EMAIL"
# Set the cache to timeout after 24 hour (setting is in seconds)
git config --global credential.helper 'cache --timeout=86400'


