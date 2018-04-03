# <i class="icon-file"></i>Linux-Command
一点点记录实用的Linux命令
   
## 终端相关基础操作  
命令|解释
--|--
tty				|查看当前所处终端  
history 50 |能看到最近50步的操作命令信息  
reset              |终端清屏  
clear              |终端清屏，保留历史，上翻记录还在      
pwd                |显示工作路径   

## 系统属性相关
命令|解释
--|--
top    |
vmstat    |
netstat -anpl | 显示系统网络状态信息，可用grep查询特定端口状态
ps -fu "username"    | 显示当前用户下所以进程
crontab | 系统定时任务,-l查看,-e编辑  

## 文件和目录相关    
命令|解释
--|--
ls               |查看目录中文件列表，参数-a(增加显示隐含目录),-l(其中，蓝色：目录，绿色：可执行文件,红色：压缩文件,浅蓝：链接文件，灰色：其他文件，红底白字：错误的链接文件)，默认按照字符升序排序，-r：按字符降序，-t：按修改时间降序，ll -t&#124;tac：按修改时间升序，-S按大小降序，ll -S &#124; tac：按大小升序  
ls -l &#124; grep "^d" &#124; wc -l  |统计当前目录下文件夹的个数
ls -lR 2018*/ &#124; grep "^-" &#124; wc -l  |统计当前目录下特定目录下文件个数，R表示包含子文件夹  
mkdir filename1  |在当前目录创建文件夹  
cp file1 file2   |拷贝文件1命名为文件2 
vi               |打开或新建文件,shift+g至文件底端,ctrl+b向上翻页,ctrl+向下翻页  
i 或者 a 或者 o   |在文件编辑模式下可开启插入模式，append(追加)insert(插入)o重起一行输入  
:wq!             |保存并强制退出文件的编辑  
more filename    |浏览文件内容  
less filename    |浏览文件内容  
tail -f filename |从尾部查看文件，并动态刷新内容  
grep "keyword" filename |查询显示含有关键词的所有行内容  
grep -v "keyword" filename |查询显示不包含关键词的所有行内容
grep -c "keyword" filename |查询统计含有关键词的行数
cat -n filename  |显示文件内容和行数  
cat -A filename  |显示不可打印字符，行尾显示"$"  
mv |重命名文件或者移动文件  
tar -czvf newfile oldfile --exclude *.log | 打包并压缩文件,不包含日志文件夹
rm a.txt         |删除文件  
rmdir filename   |在当前目录中删除该空文件夹  
rmdir -rf filename |在当前目录下直接删除非空目录，-r: 向下递归，不管有多少级目录，一并删除，-f: 直接强行删除，不做任何提示   
du | 默认列出当前目录下所有文件和文件夹占空间大小及总大小. du -sh * 显示当前目录下所有内容所占磁盘大小
    
## 用户相关
命令|解释
--|--
w或者who  |查看系统中所有登陆的用户  
logname   |当前登录用户名称  
cat /etc/passwd &#124; cut -f1 -d :  |查看系统所有用户  
useradd username | 添加用户  
passwd userpwd | 设置用户密码  

## 应用相关
命令|解释
--|--
ldd  |打印程序或应用所依赖的共享库列表
    
## 开关机相关
命令|解释
--|--
shutdown -h now |立即关机，root用户使用  
shutdown -r     |重启  
init 0          |立即关机，root用户使用  
halt            |关机，非root用户可以使用  
poweroff        |关机，非root用户可以使用            
