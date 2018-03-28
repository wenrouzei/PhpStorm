# window使用phpstorm调试xdebug

## 下载安装添加`xdebug`扩展

<a target="_blank" href="https://xdebug.org/download.php">https://xdebug.org/download.php</a>

## 修改php.ini文件配置
```
[xdebug]
zend_extension="G:\xampp\php\ext\php_xdebug.dll"
xdebug.profiler_append = 0 
xdebug.profiler_enable = 1 
xdebug.profiler_enable_trigger = 0 
xdebug.profiler_output_dir = "G:\xampp\tmp"
xdebug.profiler_output_name = "cachegrind.out.%t-%s"
xdebug.remote_enable = On 
xdebug.remote_handler = dbgp  
xdebug.remote_host= localhost  
xdebug.remote_port = 9000 
xdebug.idekey = PHPSTORM
```