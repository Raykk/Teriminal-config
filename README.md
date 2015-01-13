# Mac terminal configure

1. 通过终端偏好设置，选择配色和字体。
2. 配置文件 bash_profile(提示符颜色，以及打开ls命令的高亮显示)。

    在用户主目录下建立一个配置文件即可：
        vim ./.bash_profile

    然后写入（按i进入编辑模式）如下配置文件：
```
# for color
export CLICOLOR=1
# \h:\W \u\$
export PS1='\[\033[01;33m\]\u@\h\[\033[01;31m\] \W\$\[\033[00m\] '
# grep
alias grep='grep --color=always'
```
