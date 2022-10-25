## Linux目录
### 1.目录结构
<font color="red"> /bin </font> : 二进制可执行文件 <br>
/dev : 设备特殊文件 <br>
<font color="red"> /etc </font> : 系统管理和配置文件 <br>
<font color="red"> /home </font> : 用户主目录的基点 <br>
/lib : 标准程序设计库，动态链接库 <br>
/sbin : 超级管理命令 <br>
/tmp : 公共的临时文件存储点 <br>
<font color="red"> /root </font> : 系统管理员主目录 <br>
/mnt : 文件系统挂载目录 <br>
/proc : 虚拟的目录，系统内存的映射. 可以访问这个目录获取系统信息 <br>
/var : 某些大文件的溢出区 <br>
/usr : Unix System Resource
<br>

### 2.目录操作
`pwd` : 显示当前工作目录的绝对路径 <br>
`ls/ll/ll-a` : 列举当前目录下的目录(文件夹)和文件 <br>
`cd` : 进入到某一目录 <br>
`mkdir` : 创建文件夹 <br>
`rmdir` : 删除文件夹 <br>

### 3.文件操作
>Linux系统中一切皆文件
<br>

`touch` : 创建文件 <br>
`cp` : 复制文件/文件夹 <br>
`cp -r` : 递归复制，多级目录 <br>
`mv` : 移动文件夹/重命名 <br>
`rm` : 删除文件 <br>
`rm -rf` : 强制删除文件不需要确认 <br>
`cat` : 查看文件，一次性把文件的所有内容显示出来 <br>
`more` : 查看文件，一部分一部分的去进行显示文件内容 <br>
`less` : 查看文件，可以进行一部分的内容显示同时通过命令进行查找操作 <br>
`echo` : 输出 <br>
`head` : 查看文件头部，默认前10行 <br>
`tail` : 查看文件末尾 <br>
`tail -f` : 实时查看文件末尾 <br>
`>` : 覆盖 <br>
`>>` : 追加 <br>

### 4.文本处理类
<b>wc</b> <br>
` wc [OPTION]... [FILE]... `<br>
` wc [OPTION]... --files0-from=F` <br>
&nbsp;&nbsp;-l : --lines 统计行数 <br>
&nbsp;&nbsp;-c : --bytes 统计字节数 <br>
&nbsp;&nbsp;-w : --words 统计单词数 <br>
&nbsp;&nbsp;-L : --max-line-length 打印最长行的长度 <br>

<b>cut</b> <br>
` cut [OPTION]... [FILE]...` <br>
&nbsp;&nbsp;-d : 分隔符，按照指定分隔符分割列。与 -f 一起使用 <br>
&nbsp;&nbsp;-f : 依据 -d 的分隔字符将一段信息分割成为数段，用 -f 取出第几段的意思（列号，提取第几列） <br>
&nbsp;&nbsp;-c : 以字符 (characters) 的单位取出固定字符区间 <br>
&nbsp;&nbsp;-b : 以字节为单位进行分割 <br>

<b>sort</b> <br>
` sort [OPTION]... [FILE]...` <br>
` sort [OPTION]... --files0-from=F` <br>
&nbsp;&nbsp;-b --ignore-leading-blanks: 忽略前导空格 <br>
&nbsp;&nbsp;-f --ignore-case: 将小写字符转为大写字符 <br>
&nbsp;&nbsp;-t --field-separator=SEP: 使用SEP代替非空到空的转换 <br>
&nbsp;&nbsp;-k --key=POS1[,POS2]: 在POS1处开始键(原点1)，在POS2处结束键(默认行结束) <br>
&nbap;&nbsp;-u --unique: 对于-c检查严格的顺序，只输出相等运行的第一个 <br>

### 5.VI编辑器
##### Vi三种基本工作模式
* <font color="red">命令模式</font>
* <font color="red">文本输入模式</font>
* <font color="red">末行模式</font>

##### Vi基础操作
<b>进入插入模式</b> <br>
`i : 插入光标前一个字符` <br>
`I : 插入行首` <br>
`a : 插入光标后一个字符` <br>
`A : 插入行末` <br>
`o : 向下开新一行，插入行首` <br>
`O : 向上新开一行，插入行首` <br>
<b>进入末行模式</b> <br>
`在命令模式下，用户按“:”键即可进入末行模式` <br>
<b>退出</b> <br>
`:q : 退出` <br>
`:q! : 退出并不保存` <br>
`:w : 保存` <br>
`:wq : 保存并退出` <br>
`:wq! : 保存并强制退出` <br>
`:a : 插入光标后一个字符` <br>
`:x : 保存并退出` <br>
<b>查找命令</b> <br>
`/:str 查找` `n: 下一个` `N: 上一个` <br>


