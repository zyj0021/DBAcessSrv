# DBAcessSrv
数据库操作访问
----------------------

.NET Core实现
   服务端提供多种数据库，将常用数据库封装。NetCSDB.dll是控制台服务。启动即可。
   客户端有测试，已经封装了客户端使用。
   
实现说明
----------------------------------------------------------
1.采用ZMQ的TCP通信  
2.服务端由配置文件设置IP和端口。Server.cfg文件，放置在Config的目录  
3.封装了berkeley db数据库，Redis数据库，sqlite数据库。  
4.一般数据库采用了自定义的数据库连接池Hikari来实现服务。可以根据配置名称访问多个数据库  
5.采用Messagepack序列化  
6.程序测试默认通信地址127.0.0.1:7777  


   
