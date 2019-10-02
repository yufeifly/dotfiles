# It is the configurations of zsh.

## Install zsh & its basic configurations:  
1. sudo apt install zsh
2. chsh -s /bin/zsh (without sudo)
3. sudo vim /etc/passwd, change the first line "/bin/bash" to "/bin/zsh"

## Install oh-my-zsh:  
wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | sh

## The plugins I use:  
1. git
2. z
3. zsh-syntax-highlighting (need to git clone the corresponding repo)  
	git clone git://github.com/zsh-users/zsh-syntax-highlighting ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
4. zsh-autosuggestions (need to git clone the corresponding repo)  
	git clone git://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

## Run the following command to make it work:
source ~/.zshrc
