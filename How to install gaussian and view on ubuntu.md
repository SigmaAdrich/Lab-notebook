#在ubuntu上安装gaussian和gaussian view  
##安装包下载  
下载地址(http://pan.baidu.com/s/1i3oq79j) 密码：dd4s  
有win linux 下的资源，很全，也有gaussion view的资源,我就漏看了，浪费了好多时间  
打开linux文件夹，有好多版本，分别是09和03版的，很多种压缩包，我用的是gaosi09-D01.zip这个安装包  
#####小白科普部分，大神跳过  
讲道理呢，linux一般是用bz和.gz的安装包，不过我用的ubuntu16了，zip的也能解压。  
还要注意你的系统是64位还是32位的，对应的要下载64位或32位的安装包。从压缩包的名字里的64或者32能鉴别出来。  
##gaussian安装    
1.将压缩包解压后的文件夹命名为g09，不过一般解压出来的名字就是g09。这里重命名是为了下面敲指令的时候统一。  
2.假设我们将解压出来的文件放到了/home/usr/下,进入g09文件夹，建立一个名为scratch的文件夹，并且将其权限改为777。  这里的usr可能会不一样，需要看你的登录时候系统的名字。  
3.在home目录下，Ctrl+H，显示隐藏的文件，打开.bashrc文件，在最后加上下面的语句：  
 ##gaussian 09 start###################这是注释部分，你可以随意写东西  
export g09root=/home/usr         #这里是你的gaussian文件存放的位置  
export GAUSS_SCRDIR=/home/usr/g09/scratch  #G09 Scratch文件目录,可以随意填写位置  
source $g09root/g09/bsd/g09.profile    #G09环境变量设置  
 ##gaussian 09 end#####################这里也是注释，就是方便以后修改  
4.保存文件，退出  
5.在命令行中运行source ~/.bashrc  
6.重新登录下，在命令行中运行g09  
  
  
  这里会遇到各种问题，仔细看报错信息，一般都是找不到文件，或者权限不够，自己搜索基本都能解决，就是费事。



