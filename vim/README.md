# configurations
It is my configurations of vim.

## 1. To use .vimrc, you should first install vundle.
Vundle is a software to help you manage the plugins.  
	git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

## 2. enter into the VIM page :  
	vim  

## 3. after that, you should run:  

	PluginInstall  
to install the plugins managed by vundle. 

## 4. other
For some special plugins, you should do more than above operations.

### vim-go
Enter :GoInstallBinaries in vim page. This will download all the dependancies. Make sure that you have VPN or VPS. 

## 5. easy way to configure for all users
Thanks to the source command, we can only have one copy of vimrc file. For a user, we create a .vimrc file in his HOME directory and write only one line "source /the/path/to/.vimrc" in it.
