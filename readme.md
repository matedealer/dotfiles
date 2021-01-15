# README
Source: [Dotfile tutorial](https://www.atlassian.com/git/tutorials/dotfiles)

```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
alias config='/usr/bin/git --git-dir=$HOME/.cfg/ --work-tree=$HOME'
echo ".cfg" >> .gitignore
git clone --bare https://github/matedealer/dotfiles $HOME/.cfg
config stash
config checkout
config config --local status.showUntrackedFiles no
config status
```
