### Where use it
    
* **system requirements：**vim 7.1 or higher，support linux、 mac、 cygwin.
* **feature：**browse c/c++, python project and improve experience to modify config file
* **difference：**one command to install and it's experience is as much as source insight.


### How to install and update

* **centos, redhat, fedora install command:**
    * yum install ctags cscope wget unzip -y && wget https://github.com/jiangeZh/vim-ide/archive/master.zip -O master.zip && unzip -o master.zip && \cp -rf vim-ide-master/.vim* ~ ; rm -rf master.zip vim-ide-master
* **debian, ubuntu install command:**
    * apt-get install ctags cscope wget unzip -y && wget https://github.com/jiangeZh/vim-ide/archive/master.zip -O master.zip && unzip -o master.zip && \cp -rf vim-ide-master/.vim* ~ ; rm -rf master.zip vim-ide-master
* **mac install command, insure has installed brew, wget and unzip:**
    * brew install ctags cscope -y && hash ctags cscope wget unzip && wget https://github.com/jiangeZh/vim-ide/archive/master.zip -O master.zip && unzip -o master.zip && \cp -rf vim-ide-master/.vim* ~ ; rm -rf master.zip vim-ide-master


### How to use it read and write c/c++ project

* **open project:**
    * cd into project root dir，vim (press enter button). press F2 to open file tree, and select file to open.
* **update index:**
    * when first time open project, press F5 to update index. the index function is same to source insight index.
* **read c/c++ code:**
    * **jump**
        * **"F3":**         throught tagbar to jump to another function in the file
        * **"gd":**         jump to local varibale defination
        * **"ctrl-]":**     jump to variable or function defination in project。(can't jump to local variable defination) (:ts word)
        * **"[[":**         jump to start of function
        * **"][":**         jump to end of function
        * **"ctrl-o":**     jump to cursor last position
        * **"ctrl-i":**     return after press ctrl-o
        * **"ctrl-h":**     move cursor to left window in vim
        * **"ctrl-j":**     move cursor to down window in vim
        * **"ctrl-k":**     move cursor to up window in vim
        * **"ctrl-l":**     move cursor to right window in vim
    * **search**
        * **"ctrl-[ s":**   search variable or function in project (:cs find s word)
        * **"ctrl-[ t":**   search text in project (:cs find t word)
        * **"F7":**         highlight word under the cursor 
        * **"/word":**      search word in the file
    * **open another file in project**
        * **"F2":**         throught file tree
        * **"F8":**         throught opened file list
        * **"F4":**         switch of include file and implement file
    * **display**
        * **"F6":**         switch of display invisible character or not 
        * **"F10":**        change tab display as space mount
* **write c/c++ code：**
    * **align**
        * **"=":**          align selected code
    * **comment**
        * **",":**          comment selected code
        * **".":**          uncomment selected code
    * **replace**
        * **":%s /word1/word2/g":**  replace word1 to word2 in the file
    * **expand tab to space or not**
        * **"F9":**         exapnd tab to space or not


### Hope

* consuming less finger, less brain and less cpu to read and write code.


### Links

* vim官方网站
    * www.vim.org
* 最官方、最全、最新的下载vim脚本插件的地方
    * http://www.vim.org/scripts/index.php
* vim基本快捷键等
    * vim里使用man命令     http://blog.csdn.net/langsim/article/details/46592761
    * vim 技巧小结         http://9014348.blog.51cto.com/9004348/1640979
    * 提升效率的若干Vim技巧  http://www.dutor.net/index.php/2011/09/efficient-vim-tips/
    * Vim技巧总结          http://qindamoni.com/blog/2015/01/13/vimji-qiao-zong-jie/
    * VIM快捷键大全        http://bbs.jcwcn.com/thread-201082-1-1.html
    * 快速提高 Vi/Vim 使用效率的原则与途径   http://www.ibm.com/developerworks/cn/linux/l-cn-tip-vim/
    * 鸟哥 第九章、vim 程式編輯器            http://linux.vbird.org/linux_basic/0310vi.php
    * 高效率编辑器 VIM－操作篇               https://linuxtoy.org/archives/efficient-editing-with-vim.html
* 与这个项目类似功能的项目会配置文件说明
    * use_vim_as_ide                      https://github.com/yangyangwithgnu/use_vim_as_ide
    * 超强vim配置文件                     https://github.com/ma6174/vim
    * Vim as a Python IDE                 https://github.com/mbrochh/vim-as-a-python-ide
    * 强大的vim配置文件,让编程更随意      http://www.cnblogs.com/ma6174/archive/2011/12/10/2283393.html
    * 史上最强的Vim 配置文件              http://blog.csdn.net/redguardtoo/article/details/1172136
    * 我的VIM配置及说明K-VIM              http://www.wklken.me/posts/2013/06/11/linux-my-vim.html
    * Vim配置文件全平台可用               http://www.oschina.net/code/snippet_103341_10313
    * 将你的Vim 打造成轻巧强大的IDE  http://yuez.me/jiang-ni-de-vim-da-zao-cheng-qing-qiao-qiang-da-de-ide/
    * vim 配置文件                        http://blog.sciencenet.cn/blog-683919-667321.html
* 百科类vim说明
    * 维基百科             https://zh.wikipedia.org/wiki/Vim
    * 百度百科             http://baike.baidu.com/subview/113188/9338173.htm
* vim相关论坛门户
    ubuntu论坛vim/emacs页  http://forum.ubuntu.org.cn/viewforum.php?f=68
    * Vimer的程序世界        http://www.vimer.cn/
    * vim百度贴吧            http://tieba.baidu.com/f?kw=vim&fr=wwwt
    * 水木vim板块            http://www.newsmth.net/nForum/#!board/VIM
    * 知乎vim                http://www.zhihu.com/topic/19570193?page=2
    * 豆瓣vim                http://www.douban.com/group/vim/


### Faq

* 怎么把光标移动到左边的文件树窗口或右边的函数列表窗口?
    * ctrl-h是向左边的窗口移动,ctrl-l是向右边的窗口移动
* 问什么不让行号默认显示？
    * 右下角已经有了，不仅有行号，还有列号。
* 按tab键默认输入4个空格还是一个tab?
    * 按tab键会输入4个空格，默认的行首缩进也是4个空格。如果项目要求是行首缩进是一个tab,将配置文件set expandtab改为set noexpandtab。
* tagbar怎么没有颜色了，默认的有？
    * 给去掉了，tagbar的颜色是会在文件输入时，时时运行正则表达式，会在自动补全时拖慢速度。
* 自动补全列表怎么选择，怎么确认最好？
    * 按上下键选择，按回车键补全。
* 自动补全列表只有在输入. -> :: 时才弹出?
    * 在输入一半单词时，按tab也会弹出。
* 相当于windows里的ctrl-z的撤销，在vim里怎么做？
    * u是撤销，ctrl-r是重做。
* 之前也用ctags、cscope,使用命令更新索引，这个F5更新索引与是用命令的区别是什么？
    * vim用这个配置文件时，F5快捷键会把ctags，cscope两个索引都更新了，不用再输入那两个命令了。
* 打开一个工程，已经更F5新好索引，怎么跳转main函数？
    * :ts main
* 怎么对齐nginx的配置文件？
    * gg=G可以对其整个文件，但vim默认配置对齐后会让注释行没有缩进。用这个配置文件没有这个问题。
* vim的复制粘贴？
    * 先按v或shift-v，选中一些内容，按y复制，把光标移动到想要粘贴的位置，按p。
* 为什么没有把youcompleteme集成进来？
    * 我的评估结果是，他的复杂度大于实用度。而且现在的补全我觉得已经太够用了。
* diff命令或svn diff命令出来的东西没有语法着色？
    * diff ***** | vim - 或
    * svn diff **** | vim -
    * 当然其他输出到终端的东西加上 | vim -也可以。
    * '|'的意思是把上个命令的stdout，作为下一个命令的stdin。
    * '-'的意思是把stdin作为一个文件打开
* 这个配置文件在搜索跳转补全等方面对c++支持怎么样？
    * 非常好
* vim用了这个配置文件后跟sourceinsight等工具对比怎么样？
    * souce insight:通过Linux上的samba服务去写Linux主机里的代码，或者在windows上用source insight写完代码后再传到linux上。
    * eclipse:很好用，但不得打开Linux图形界面，另外eclipse运行很慢，尤其大项目。
    * qt creator:即使不是QT项目，当然也可以在Linux图形界面用QT creator写代码，比eclipse运行快。
    * codeblocks:也跟eclipse和qtcreator一样,要在linux下的图形界面下使用，用的不多，不做评价。
    * VIM与EMACS:作为开发环境都要加跳转及自动补全类的插件。它们都可以直接ssh到Linux主机直接使用,不需要打开图形界面。VIM与EMACS都可以无界限的加任何功能的插件。从基本操作上个人还是更喜欢emacs，但vim更容易定制到自己希望的样子。
* 这份配置文件里用了哪些vim插件，这些插件是否是原生的?
    * tagbar         #函数变量列表（修改部分BUG，修改配置文件）
    * nerdcommenter  #注释功能（修改C语言默认用//注释，修改配置文件）
    * a              #切换头文件和实现文件（修改跨目录不能找到的问题，无修改配置文件）
    * nerdtree       #目录树（无修改，修改配置文件）
    * omnicpp        #C/C++的自动补全插件（无修改，修改配置文件）
    * bufexplorer    #当前打开的文件列表（无修改，修改配置文件）
    * AutoComplPop   #自动弹出补全菜单 （无修改，无修改配置文件）
* 安装命令都做了什么？
    * 安装cscope, ctags, 然后下载一份vim脚本放在家目录下，最后清除临时文件。
