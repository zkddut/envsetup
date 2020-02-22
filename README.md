# envsetup
Note for envsetup

# vim install
https://www.poftut.com/how-to-download-and-install-gvim-for-windows-ubuntu-mint-centos-fedora/
```
sudo apt install vim-gtk
```

# Shell install
> install zsh
https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH


> change to ohmyzsh
https://github.com/ohmyzsh/ohmyzsh

> change setting in .zshrc using pure
https://github.com/sindresorhus/pure
```
.zshrc change
fpath+=$HOME/.zsh/pure
autoload -U promptinit; promptinit
prompt pure
zstyle :prompt:pure:path color white

```

# vimrc install
https://github.com/amix/vimrc
```
git clone --depth=1 https://github.com/amix/vimrc.git ~/.vim_runtime
sh ~/.vim_runtime/install_awesome_vimrc.sh
change in .vimrc
set guifont=Monospace\ 10
set tabstop=2
set softtabstop=0 noexpandtab
set shiftwidth=2

```
> easy to forget vim commond
```
<leader> -> ,

open a new windown: <Ctrl>+<w> <v>/<s>
move to a new windown: <Ctrl>+<w> <up>
		increase the width of your window by pressing <Ctrl>+<w> and then ‘>’/'+'/'='

Fuzzy file, buffer, mru and tag finder. It's mapped to <Ctrl+F>
open a file in current folder :open
open current folder :Explore
change directory to current buffer <leader> cd

NERD Tree: map <leader>nn :NERDTreeToggle<cr>; map <leader>nf :NERDTreeFind<cr>
? open help for NERD tree

Open file under cursor when pressing gf
Switch buffer <leader> o / q exit
MRU: most recently use <leader> f	
quickly find a file or a buffer (<leader>j or <ctrl>f):

```

# terminal multiplexer
https://linuxize.com/post/getting-started-with-tmux/
```
sudo apt install tmux
```


# alias
```
alias ll='ls -alF'
alias la='ls -A'
alias l='ls -CF'
alias g='gvim'
alias lk='find . | grep'
alias fs='grep -irn'
alias ..='cd ..'
function fk() {
  lk $1 | xargs grep $2;
}
function mkd() {
  mkdir $1; cd $1;
}
```

# Add ssh key for github
https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

