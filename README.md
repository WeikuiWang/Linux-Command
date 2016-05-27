# Linux-Command
从零开始一步一步记忆最实用的Linux命令
## 3/12/2016 start!
此次编辑的数十个命令是笔者近几天积累的一些最基础命令，一些命令参数可能描述不全，另如有失误之处请指正.

    右键 然后 e         在liunx桌面打开终端
    python              进入python交互模式
    Ctrl+d              若在交互模式，退出python交互模式，若在系统界面，则关闭终端
    tty                 查看当前所处终端
    w或者who            查看系统中所有登陆的用户
    cd /home            进入home目录
    cd ..               返回上级目录
    pwd                 显示工作路径
    ls                  查看目录中文件列表，参数-s,-a(增加显示隐含目录),-l(其中，蓝色：目录，绿色：可执行文件，红色：压缩文件，浅蓝：链接文件，灰色：其他文件，红底白字：错误的链接文件)
    mkdir filename1     在当前目录创建文件夹
    rmdir filename      在当前目录中删除该空文件夹
    rmdir -rf filename  在当前目录下直接删除非空目录，-r: 向下递归，不管有多少级目录，一并删除，-f: 直接强行删除，不做任何提示
    vi                  打开或新建文件
    xdg-open a.txt      打开a.txt文件，用相应的应用程序打开
    :wq!                保存并强制退出文件的编辑
    rm a.txt            删除文件
    shutdown -h now     立即关机，root用户使用
    init 0              立即关机，root用户使用
    halt                关机，非root用户可以使用
    poweroff            关机，非root用户可以使用
    i 或者 a 或者 o     在文件编辑模式下可开启插入模式，append(追加)insert(插入)o重起一行输入
    python              在终端进入python交互模式
    history 50          能看到最近50步的操作命令
    cp filename1 filename2   拷贝文件1命名为文件2
    reset               终端清屏
    clear               终端清屏，保留历史，上翻记录还在
    more filename       浏览文件内容，默认80%的内容
    less filename       浏览文件内容
    find  文件或目录名   查找文件，目录的话列出其子目录信息
    mv 文件或文件名1 文件或文件名2    重命名文件1为文件2
    tar xvf 压缩文件名带后缀     加压某文件
