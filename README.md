# TIPS

## Ⅰ.pyinstaller
>[the use of pyinstaller](https://blog.csdn.net/qq_34106574/article/details/82964110)  
-F, &nbsp; –onefile	产生一个文件用于部署 (参见XXXXX).  
-D, &nbsp;–onedir	产生一个目录用于部署 (默认)
-K, &nbsp;–tk	在部署时包含 TCL/TK  
-a, &nbsp;–ascii	不包含编码.在支持Unicode的python版本上默认包含所有的编码.  
-d, &nbsp;–debug	产生debug版本的可执行文件  
-w,–windowed,–noconsole	&nbsp;使用Windows子系统执行.当程序启动的时候不会打开命令行(只对Windows有效)  
-c,–nowindowed,–console	&nbsp;使用控制台子系统执行(默认)(只对Windows有效)  
-s,–strip	&nbsp;可执行文件和共享库将run through strip.注意Cygwin的strip往往使普通的win32 Dll无法使用.  
-X, –upx	&nbsp;如果有UPX安装(执行Configure.py时检测),会压缩执行文件(Windows系统中的DLL也会)(参见note)  
-o DIR, –out=DIR	&nbsp;指定spec文件的生成目录,如果没有指定,而且当前目录是PyInstaller的根目录,会自动创建一个用于输出(spec和生成的可执行文&nbsp;件)的目录.如果没有指定,而当前目录不是PyInstaller的根目录,则会输出到当前的目录下.  
-p DIR, –path=DIR	&nbsp;设置导入路径(和使用PYTHONPATH效果相似).可以用路径分割符(Windows使用分号,Linux使用冒号)分割,指定多个目录.也可以使用多&nbsp;个-p参数来设置多个导入路径  
–icon=<FILE.ICO>	&nbsp;将file.ico添加为可执行文件的资源(只对Windows系统有效)  
–icon=<FILE.EXE,N>	&nbsp;将file.exe的第n个图标添加为可执行文件的资源(只对Windows系统有效)  
-v FILE, –version=FILE	&nbsp;将verfile作为可执行文件的版本资源(只对Windows系统有效)  
-n NAME, –name=NAME	&nbsp;可选的项目(产生的spec的)名字.如果省略,第一个脚本的主文件名将作为spec的名字  
