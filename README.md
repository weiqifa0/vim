# 超强vim配置文件

[![Build Status](https://travis-ci.org/ma6174/vim.png?branch=master)](https://travis-ci.org/ma6174/vim)

### 运行截图

![screenshot.png](screenshot.png)

### 简易安装方法：

打开终端，执行下面的命令就自动安装好了：

`wget -qO- https://raw.github.com/ma6174/vim/master/setup.sh | sh -x`
`wget -qO- https://github.com/weiqifa0/vim/master/setup.sh | sh -x`

### 或者自己手动安装：(以ubuntu为例)

1. 安装vim `sudo apt-get install vim`
- 安装ctags：`sudo apt-get install ctags`
- 安装一些必备程序：`sudo apt-get install xclip vim-gnome astyle python-setuptools`
- python代码格式化工具：`sudo easy_install -ZU autopep8`
- `sudo ln -s /usr/bin/ctags /usr/local/bin/ctags`
- clone配置文件：`cd ~/ && git clone git://github.com/ma6174/vim.git`
- `mv ~/vim ~/.vim`
- `mv ~/.vim/.vimrc ~/`
- clone bundle 程序：`git clone https://github.com/gmarik/vundle.git ~/.vim/bundle/vundle`
- 打开vim并执行bundle程序`:BundleInstall`
- 重新打开vim即可看到效果

### 了解更多vim使用的小技巧：

[tips.md](tips.md)

### 查看更新日志：

[`update_log.md`](update_log.md)

## 总结使用的心得。
* ctags -R * 用来生成tags
* set paste 设置后，右键粘贴就不会自动注释。
* shift + “*” 向下查找并高亮显示
* shift + “#” 向上查找并高亮显示
* “g” + “d” 高亮显示光标所属单词，“n” 查找！

# vim 使用tip

### 编写python程序

1. 自动插入头信息：
    - `#!/usr/bin/env python`
    - `# coding=utf-8`
- 输入`.`或按`TAB`键会触发代码补全功能
- `:w`保存代码之后会自动检查代码错误与规范
- 按`F6`可以按`pep8`格式对代码格式优化
- 按`F5`可以一键执行代码


### 多窗口操作

1. 使用`:sp + 文件名`可以水平分割窗口
- 使用`:vs + 文件名`可以垂直分割窗口
- 使用`Ctrl + w`可以快速在窗口间切换

### 编写markdown文件

1. 编写markdown文件(`*.md`)的时候，在normal模式下按 `md` 即可在当前目录下生成相应的`html`文件
- 生成之后还是在normal模式按`fi`可以使用firefox打开相应的`html`文件预览
- 当然也可以使用万能的`F5`键来一键转换并打开预览
- 如果打开过程中屏幕出现一些混乱信息，可以按`Ctrl + l`来恢复

### 快速注释

- 按` \ ` 可以根据文件类型自动注释


## ctags基本命令
* $ctags –R * ($为Linux系统Shell提示符,这个命令上面已经有所介绍)
* $ vi –t tag (请把tag替换为您欲查找的变量或函数名)
* :ts(ts助记字：tagslist, “:”开头的命令为VI中命令行模式命令)
* :tp(tp助记字：tagspreview)---此命令不常用，可以不用记
* :tn(tn助记字：tagsnext) ---此命令不常用，可以不用记
* Ctrl+ ]跳到光标所在函数或者结构体的定义处
* Ctrl+ T返回查找或跳转

# VIM快捷键汇总
http://mp.weixin.qq.com/s?__biz=MzA5NTM3MjIxMw==&mid=100003543&idx=1&sn=5b888479a83888f72776cba8999a845e&chksm=1041180d2736911b40f52e8c2eb949437a3b5b05e02d9aa41a449f09bbec7d63fa1a082050d9#rd

