# Dotfiles

Here are my dotfiles, I will be adding to it and explaining along the way.

A journey begins.

## Setup/

### HomeBrew related
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
ln -s ~/Documents/Github/dot_files/.Brewfile ~/.Brewfile
brew bundle --global
```

### Symlinks
```
stow conda hammerspoon karabiner nvim pdb rich ssh tmux zsh
```

### Additional steps

- Karabiner :
    - Open Karabiner-Elements from your Applications folder.
    - Grant necessary permissions in System Preferences > Security & Privacy (Input Monitoring and Accessibility). 

- Postgres related :
```
createuser --superuser $USER -U postgres
createdb $USER -U $USER
```