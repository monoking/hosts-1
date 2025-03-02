说明
----

hosts文件是一个没有扩展名的系统文件，它的主要作用是能加快域名解析，还可以屏蔽网站等。 

持续更新Google、Gmail、谷歌学术、Google Play、Facebook、Twitter、Youtube、Android、亚马逊、雅虎、维基百科、Mozilla、Github、、Archive、Battle.NET、Box.com、BundleStars、DeviantART、DuckDuckGo、HumbleBundle、imgur、Indiegala、inoreader、Instagram、Ixquick、Logmein、MEGA、OneDrive、osu、RockStar、SoundCloud、Speedtest、Startpage、Steam、WordPress、XDA、Appannie、Travis CI fastly CDN等hosts。

工作原理
--------

浏览器访问网站，要首先通过DNS服务器把要访问的网站域名解析成一个唯一的IP地址，之后，浏览器才能对此网站进行定位并且访问其数据。

操作系统规定，在进行DNS请求以前，先检查系自己的Hosts文件中是否有这个域名和IP的映射关系。如果有，则直接访问这个IP地址指定的网络位置，如果没有，再向已知的DNS服务器提出域名解析请求。也就是说Hosts的IP解析优先级比DNS要高。

适用系统
--------
  
  * Unix
  * Linux
  * Android
  * Mac
  * Windows

更新地址
--------

提供了下面两个更新地址：

  * [hosts_免费高速下载|百度云 网盘-分享无限制](http://pan.baidu.com/s/1kTlKev9)
  * [liuker0x007/hosts - Github](https://github.com/liuker0x007/hosts)
  
使用方法
--------

### Linux & Unix
Linux 系统终端下命令：  
使用wget或curl，以wget为例：  
开启终端(快捷键为"Ctrl + Alt + T")输入`bash -c 'wget https://github.com/liuker0x007/hosts/tree/master/20151115/Linux/hosts -qO /tmp/hosts && sudo mv /tmp/hosts /etc/hosts'`
或者非命令：
打开`/etc/hosts` 目录，把下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。
<br>最后在终端输入`sudo systemctl restart NetworkManager`
<br>**注意 : 非systemd发行版，终端输入`sudo rcnscd restart`，如果不清楚请两个都试一次。**

### Android
如果是Android系统，用 RE管理器 （前提需要手机已Root）打开`/system/etc/hosts`目录，把下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。然后通过`开启飞行模式 -> 关闭飞行模式 `的方式使其生效。

### Mac
如果是Mac系统，打开你的文件管理器（也就是Finder），然后，请按快捷键组合“Shift+Command+G”三个组合按键查找文件，并输入Hosts文件的所在路径：`/etc/hosts`，把下载好的`hosts`文件粘帖和覆盖该目录的`hosts`文件。然后终端输入`sudo killall -HUP mDNSResponder`使其生效。

### Windows
用文本编辑器(如Notepad++|记事本)打开`C:\Windows\System32\drivers\etc`中的hosts文件，把 -> 下载好的`hosts`文件 <- 全部内容复制到`C:\WINDOWS\system32\drivers\etc`目录中的hosts文件中，保存后通过```开始 -> 运行 -> 输入cmd -> 在CMD窗口输入ipconfig /flushdns```使其生效。
<br>**注意：如果遇到无法保存，请右键hosts->属性->安全，然后选择你登陆的用户名，最后点击编辑，勾选"写入"即可。**

注：如果`hosts`文件中有内容，请把它追加到`hosts`文件末尾。

更新时间
--------

基本上每周周末都会更新一次。

联系方式
--------

  * E-mail：lzq@liuker.xyz
  * QQ：2523417411
