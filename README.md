# 在线聊天室(Making a Web Chat With PHP and Swoole)

------

使用swoole扩展和php开发的一个在线聊天室，**目前实现的功能有** ：

> * 支持群聊
> * 支持发送文字
> * 支持发送图片
> * 支持@人
> * 支持分房间聊天功能
> * 显示消息数

# 如何运行？

1.先将client目录放置在您的web服务器下，打开client/static/js/init.js 文件，将该文件的配置修改成自己的域名或者IP

2.打开server目录，首先将rooms目录以及其子目录权限设为777，确保该目录可写。将client/uploads目录设置为777可写。

3.修改server/config.inc.php 文件。将下面一行代码修改为您的域名或者IP。 !!!  !!! !!!

> define("DOMAIN","http://127.0.0.1:8081");

并且将下面这样修改为rooms所在的路径   !!!  !!! !!!

> define('ONLINE_DIR','/mnt/hgfs/swoole/chatroom/rooms/');

4.命令行执行 ：
> /usr/local/php/bin/php /path/server/hsw_server.php 
 
 
 
 最后：
 >-->--> 将client运行在http服务器上并打开index页面就能够进入群聊中。


# 资料说明
1. swoole官网 http://www.swoole.com

2. 程序聊天界面采用钉钉的UI方案

3. 前端使用插件：
上传图片插件 —— Plugins文件夹是一个封装好的跨域上传js控件。

4. 本程序使用的是文件存储。没有测试抗压能力，并且可能存在BUG，如有bug则将在后续有空闲时间时再进行排除。


5. 本项目采用前后段分离的思想进行构建。




---
<br><br><br><br>

<p align="right">by Alexander Ezharjan</p>
<p align="right">on 9th August,2020</p>
