# It is the configurations of zsh.

## Install zsh & its basic configurations:  
1. sudo apt install zsh
2. chsh -s /bin/zsh (without sudo)
3. sudo vim /etc/passwd, change the first line "/bin/bash" to "/bin/zsh"

## Install oh-my-zsh:  
wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | sh

运行完以上命令后会在HOME目录产生zshrc文件，后面的配置需要修改这个文件

## The plugins I use:  
1. git

2. z

3. zsh-syntax-highlighting (need to git clone the corresponding repo)  
	git clone git://github.com/zsh-users/zsh-syntax-highlighting ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
	
4. zsh-autosuggestions (need to git clone the corresponding repo)  
	git clone git://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
	
5. zsh-history-substring-search (need to git clone the corresponding repo)  

   git clone https://github.com/zsh-users/zsh-history-substring-search ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-history-substring-search
   
   在zshrc文件中加上如下的三行：

```
  plugins=(
    git
    history-substring-search
  )

  source $ZSH/oh-my-zsh.sh

  bindkey -v
  bindkey "^[[A" history-substring-search-up
  bindkey "^[[B" history-substring-search-down
```



## Run the following command to make it work:
source ~/.zshrc

