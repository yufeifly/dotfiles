# configurations
It is my repo of configurations.

## usage

1.  git clone this repo

   ```
   https://github.com/yufeixiong/dotfiles.git
   ```

2. set a global variable
   - vim /etc/profile
   - add to the end "export DOTFILES=/home/alan/dotfiles"

3. you can just source relative dotfiles in this repo 

   e.g. in ~/.vimrc , you just add **one** line "source $DOTFILES/vim/vimrc"