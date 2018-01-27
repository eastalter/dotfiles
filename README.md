# dotfiles
## Install
```
cd ~/
git clone https://github.com/eastalter/dotfiles.git
./dotfiles/link.sh
```

## zshrc

Refer to https://gist.github.com/mollifier/4979906


## Note

squid上では`.bashrc`の最下部に以下を追加

```
which zsh > /dev/null 2>&1
if [ $? -eq 0 ]; then
    echo "The existence of Zsh was confirmed"
else
    echo "The existence of Zsh was not confirmed"
    echo "Start installing Zsh"
    yes | sudo apt-get install zsh
fi
zsh
exit
```

