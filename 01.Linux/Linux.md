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

