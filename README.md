# Linux-Command
一点点记录实用的Linux命令
   
## 终端相关基础操作
tty                 查看当前所处终端  
history 50          能看到最近50步的操作命令信息  
reset               终端清屏  
clear               终端清屏，保留历史，上翻记录还在      
pwd                 显示工作路径  
   
## 文件和目录相关    
    ls                  查看目录中文件列表，参数-a(增加显示隐含目录),-l(其中，蓝色：目录，绿色：可执行文件，红色：压缩文件，浅蓝：链接文件，灰色：其他文件，红底白字：错误的链接文件)  
    mkdir filename1     在当前目录创建文件夹  
    cp file1 file2      拷贝文件1命名为文件2  
    vi                  打开或新建文件  
    i 或者 a 或者 o     在文件编辑模式下可开启插入模式，append(追加)insert(插入)o重起一行输入  
    :wq!                保存并强制退出文件的编辑  
    more filename       浏览文件内容  
    less filename       浏览文件内容  
    mv 文件或文件名1 文件或文件名2    重命名文件1为文件2  
    rm a.txt            删除文件  
    rmdir filename      在当前目录中删除该空文件夹  
    rmdir -rf filename  在当前目录下直接删除非空目录，-r: 向下递归，不管有多少级目录，一并删除，-f: 直接强行删除，不做任何提示   
    
## 用户相关
    w或者who            查看系统中所有登陆的用户  
    logname             当前登录用户名称  
    
## 开关机相关
    shutdown -h now     立即关机，root用户使用  
    shutdown -r         重启  
    init 0              立即关机，root用户使用  
    halt                关机，非root用户可以使用  
    poweroff            关机，非root用户可以使用            
