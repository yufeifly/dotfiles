# configurations
It is my configurations of vim.
Basicly, there are two configuration files.
- vimrc
- vimrc-go

## vimrc
### 1. To use vimrc, you should first install vundle.
Vundle is a software to help you manage the plugins. 

	git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

### 2. Enter into the VIM page:  
	vim 

### 3. After that, you should run to install the plugins managed by vundle. 
	PluginInstall  

### 4. other
For some special plugins, you should do extra work.

- vim-go
> Enter `:GoInstallBinaries` in vim page. This will download all the dependancies. Make sure that you have VPN or VPS. 

- easy way to configure for all users
Thanks to the source command, we can only have one copy of vimrc file. For a user, we create a .vimrc file in his HOME directory and write only one line "source /the/path/to/.vimrc" in it.

---
## vimrc-go
Vimrc for golang website: https://learnku.com/articles/24924
We now use vim-plug to manage plugins.

## install
If you are in linux environment, vim-plug installation is easy. Simply run
`curl -fLo ~/.vim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim`

Enter the vim homepage and input:
`:PlugInstall`

If you want to clean some plugins, comment them and run:
`:PlugClean`

For vim-go plugin, you need to explicitly run:
`:GoInstallBinaries`

For the installation of ycm, you need extra work too. You should get **build-essential cmake python3** installed on your machine and cd into the directory:
`cd ~/.vim/plugged/YouCompleteMe`, and run `python3 install.py --go-completer`

Also, you need some configurations to deal with the shortcut key conflict.
```
let g:ycm_key_list_select_completion = ['<C-n>', '<space>']
let g:ycm_key_list_previous_completion = ['<C-p>', '<Up>']
let g:SuperTabDefaultCompletionType = '<C-n>'

" better key bindings for UltiSnipsExpandTrigger
let g:UltiSnipsExpandTrigger = "<tab>"
let g:UltiSnipsJumpForwardTrigger = "<tab>"
let g:UltiSnipsJumpBackwardTrigger = "<s-tab>"
```
