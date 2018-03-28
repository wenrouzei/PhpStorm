# window使用phpstorm调试xdebug

## 下载安装添加`xdebug`扩展

<a target="_blank" href="https://xdebug.org/download.php">https://xdebug.org/download.php</a>

## 修改php.ini文件配置
```
[xdebug]
zend_extension="G:\xampp\php\ext\php_xdebug.dll"
xdebug.profiler_append = 0 
xdebug.profiler_enable = 0 
xdebug.profiler_enable_trigger = 1 
xdebug.profiler_output_dir = "G:\xampp\tmp"
xdebug.profiler_output_name = "cachegrind.out.%t-%s"
xdebug.remote_enable = On 
xdebug.remote_handler = dbgp  
xdebug.remote_host= localhost  
xdebug.remote_port = 9000 
xdebug.idekey = PHPSTORM
```

## 界面

>debugger 调试器

>Resume Program 恢复程序

>Restore Layout 恢复布局

>frames 帧

>Pin Tab 一个标签页

>Show Execution Point 显示执行点

>Step Over 在单步执行时，在函数内遇到子函数时不会进入子函数内单步执行，而是将子函数整个执行完再停止，也就是把子函数整个作为一步。有一点,经过我们简单的调试,在不存在子函数的情况下是和step into效果一样的（简而言之，越过子函数，但子函数会执行）

>Step Into 单步执行，遇到子函数就进入并且继续单步执行（简而言之，进入子函数）；

>Force Step Into 强行进入函数内

>Step Out 当单步执行到子函数内时，用step out就可以执行完子函数余下部分，并返回到上一层函数。

>Run to Cursor 运行到光标所在的行

>Evaluate Expression 计算表达式窗口，当需要动态查看某一个值的时候用到

>Add method to skip list 添加方法跳过列表

