---
Linux
---
###linux命令

```bash
help  +...
```
内部命令查看格式
绝对路径：以根目录（/）开头
相对路径：不以根目录（/）开头

linux操作系统核心文件：   anaconda-ks.cfg
普通用户：/home
root用户：/root
创建用户： user add


目录操作命令 pwd 查看工作目录 

```bash 
cd：    切换工作目录
格式 ：   cd  ——
ls   ：     显示目录文件内容
格式：   ls  
ls -l  以长格式显示  缩写ll
ls -a 显示目录文件的全部信息
ls -d  显示目录文件的属性
ls -color  颜色区分
蓝色为目录 黑色为文件
```

mkdir  创建新的目录
mkdir  -p  /../../..创建多级目录
```bash
 mkdir  文件名

```   



touch  新建txt文件   或者更新文件时间标记
```bash touch 文件名
```

cat  显示文件的全部内容
```bash   cat  文件名
```
 
```bash 
vim  编辑文件  
格式：  vim  文件名
退出 esc  ：  wq
！强制执行
```



rm  删除文件或者目录
删除目录加r
格式： rm  -r  目录文件名
加f强制删除
格式：rm -rf  文件名
 ```bash rm  文件名
 ```



cp 复制文件或者目录文件
复制目录文件后加r
格式：cp -r 目录文件名
```bash cp 文件名   目标文件
```



mv：移动文件或者目录文件
```bash  mv  文件   目标
```
 

less： 全屏分页显示文件内容
enter  向下逐行滚动
空格键   向下翻屏   
b  向上翻屏
q  退出
```bash less  文件名
```


```bash tar： 归档文件  释放归档文件（解压缩）
1.格式： tar -czvf 存放路径/归档文件名.tar.gz 源文件
解压格式：tar -xzvf 解压路径 -C 存放路径
2.格式：   tar -cjvf  存放路径/归档文件名.tar.bz2 源文件
解压格式：tar xjvf 解压路径 -C 存放路径-
```
find：用于查找文件目录或文件
-name  按文件名查找
-user  按文件属主查找
 -type  按文件类型查找
d： 目录           f  ： 文件
```bash find  查找范围  查找条件
```

grep：在文件夹中查找并显示包含制定字符串的行
常用命令：  -i  查找时忽略大小写
-v  反转查找   ：输出和查找不相符的行
要查找的字符串以双引号抬起来
“^……”表示以……开头的行
“……$”表示以……结尾的行
“^￥”表示空行
```bash grep 选项  查找条件  目标文件 
``` 


```bash
command > file   将输出重定向到 file。
command < file   将输入重定向到 file。
command >> file     将输出以追加的方式重定向到 file   
n > file    将文件描述符为 n 的文件重定向到 file。
n >> file    将文件描述符为 n 的文件以追加的方式重定向到 file。
n >& m   将输出文件 m 和 n 合并。
n <& m   将输入文件 m 和 n 合并。
<< tag    将开始标记 tag 和结束标记 tag 之间的内容作为输入。
```

命令别名
alias 别名="实际执行的命令“
取消已设置的命令别名
格式：unalias 别名
unalias a
使别名永久生效：保存到 /ect/bashrs 文件夹中
例如：alias a=‘cd /root/Desktop’
a就等于此命令

```bash alias  别名
```

历史命令
清除历史命令： history -c
！n执行历史记录中的第n条命令
```bash history
```


vim编辑器的工作模式：
命令模式  输入模式  末行模式
命令 ----- a  i  o  等键 ----  输入----esc----命令----：---末行---esc---命令
格式：vi  文件名
 


