# vim
Configuration for my vim environment

1. Copy `.vimrc` to the new machine as `~/.vimrc` 
2. Install [`pathogen`](https://www.vim.org/scripts/script.php?script_id=2332)
3. Install [`Vundle`](https://github.com/VundleVim/Vundle.vim)
```
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
4. Install [`nerdtree`](https://github.com/scrooloose/nerdtree) 
```
git clone https://github.com/scrooloose/nerdtree.git ~/.vim/bundle/nerdtree
```
5. Install [`NERD commenter`](https://github.com/preservim/nerdcommenter) (for using `<leader>cc` to toggle comments and block of comments): 
```
cd ~/.vim/bundle 
git clone https://github.com/preservim/nerdcommenter.git
```
Afterwards, according to my comment in `.vimrc`, I will change the default key mapping `<leader>c<space>` to `<leader>cc` for toggling comments in `NERD_commenter.vim`: 
```
\#call s:CreateMaps('nx', 'Comment',    'Comment', 'cc') 
\#call s:CreateMaps('nx', 'Toggle',     'Toggle', 'c<space>') 
call s:CreateMaps('nx', 'Comment',    'Comment', 'c<space>') 
call s:CreateMaps('nx', 'Toggle',     'Toggle', 'cc')
```
6. Install [`dirdiff`](https://github.com/will133/vim-dirdiff) (to visualize the difference between two directories):  
```
cd ~/.vim/bundle
git clone git://github.com/will133/vim-dirdiff
```

