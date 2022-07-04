## 1 Emacs 简介

* 版本 GNU Emacs
* GNU Emacs 于 1984 年，Richard Stallman 发起并维护
* 竞争对手 VIM，VSCode 等
* 跨平台，内核解释器 C 编写，通过 ELisp 语言进行拓展

## 2 Emacs 安装

### 2.1  Windows

* scoop
* choco
* 官网 www.gnu.org/software/emacs

### 2.2  Linux

使用分发版自带的包管理器

* Ubuntu: sudo apt install emacs
* Fedora: sudo dnf install emacs
* Arch: sudo pacman -S emacs
* 官网下载源码编译安装

### 2.3 macOS

* Homebrew: brew cask install emacs
* 官网下载安装

## 3 Emacs 版本

## 4 Emacs 初识

![image.png](https://pic.rmb.bdstatic.com/bjh/783533c1e5589b8e5a5dfe40ed30f477.jpeg)

绿色：菜单栏

红色：工具栏

黄色：编辑区域

蓝色：状态栏（时间、信息、行号等）

紫色：交互区域（输出信息、M-x操作等）

## 5 基本操作速记

* C，代表 CTRL 键
* M，代表 Meta 键，往往是 ALT，部分是 ESC



光标移动：

* C-n，下一行（Nextline）
* C-p，前一行（Previous  line）
* C-f，向前移动一个字符（Forward）
* C-b，向后移动一个字符（Backforward）
* C-k，从光标位置到末尾删掉（Kill）
* C-a，回到行首（a是字母表的开始）
* C-e，去到行尾（End of line）
* M-<，回到编辑区域最开始
* M->，到编辑区域最后位置
* C-v，向下翻一屏
* M-v，向上翻一屏

## 6 自带文档

* C-h t : 速记 Help Tutorial
* C-h k : 速记 Help Keybind
* C-h f : 速记 Help  Function

## 7 外观改变

* 图形化配置 M-x customize
* 菜单栏 menu-bar-mode
* 工具栏 tool-bar-mode
* 滚动条 scroll-bar-mode

优势：不用写 Elisp 代码

劣势：

* 搜索
* 生成的配置文件只能是单一配置文件
* 扩展的配置不容易进行
* 涉及到复杂逻辑不方便配置

## 8 体验用配置文件配置

windows 下在 C:\Users\leibaio\AppData\Roaming .emacs 配置内容

## 9 认识配置文件

Emacs 配置文件的位置中，会按照以下顺序查找：

* .emacs
* .emacs.d
* emacs/init.el

第一个是一个单一配置文件；第二个更符合工程化；第三个仅适用于 27 版本及以上

## 10 为什么不用大牛配置

* 大牛配置：Spacemacs、Centaur Emacs、Doom Emacs、Steve Purcell、redguidetoo...
  * 兼容性好
  * 代码质量高
  * 功能齐全
  * 开箱即用
* 为什么不用
  * 体验配置 Emacs  的乐趣
  * 体验大牛成长的过程
  * 追求轻量、速度、新

## 11 第一行 Emacs 配置代码