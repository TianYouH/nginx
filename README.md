## 命令

### windows 下

[初学者指南](http://nginx.org/en/docs/beginners_guide.html)

[windows文档](http://nginx.org/en/docs/windows.html)


简书
>[nginx安装](https://www.jianshu.com/p/0f2cd118fd45)

>[nginx基础](https://www.jianshu.com/p/d0f9ce48e3c3)




启动进程
  
    方法一: 双击exe;
    方法二：执行文件本目录下 命令`start nginx.exe`;

查看进程

    `tasklist /fi "imagename eq nginx.exe"`;

结束进程

    方法一：`taskkill /pid {pid}`;
    方法二：`taskkill /im nginx.exe /f`; /f 在这里意为强制结束进程;
    方法三：`nginx.exe -s stop`; 强制停止
    方法四：`nginx.exe -s quit`; 正常停止

进程重启

    `nginx -s reload` 更改配置，使用新配置启动新辅助进程，使旧辅助进程正常关闭

重开日志

    `nginx -s reopen`; 重新打开日志文件