# 安装与配置

- 直接使用apt安装

> sudo apt install tmux

- 配置文件在~/.tmux.conf

> 如果没有这个文件，就创建一个。
>
> 可以将本项目中的.tmux.conf文件中的内容复制到对应文件。

- 生效

> tmux source ~/.tmux.conf



# 使用技巧

## 复制粘贴

在tmux.conf中增加*set-window-option -g mode-keys vi*，

ctrl + a + [ 进入复制模式，然后space开始选择，enter键停止选择。

ctrl + a + ] 粘贴。