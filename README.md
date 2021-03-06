# Socket_chat

tags: socket QT

* [1.开发平台](#h1)
* [2.基本功能](#h2)
* [3.实现原理](#h3)

<h1 id="h1"> 开发平台 </h1>
>   基于QT5.8.0 MINGW版本开发
    运行环境为win 64bit

<h1 id="h2"> 基本功能 </h1>
    1. 工具包括服务器端和客户端；</br>
    2. 具备用户注册、登录、找回密码功能（基于TCP协议）；
    3. 两个用户如果同时在线，采用点到点通信方式进行聊天，信息不需要通过服务器中转，服>务器也不保存（基于TCP协议）；
    4. 支持离线消息（基于TCP协议）；
    5. 支持点到点可靠文件传输（基于UDP协议）；
    6. 存储在服务器端的数据需要进行强加密；
    7. 支持不少于两组用户同时在线交流和传输文件；
    8. 文件传输具有良好的性能，能够充分利用网路带宽；

# 预期实现功能

> + 服务器端在linux机器上完成，部署到云主机上
>
> + 服务器进程做成主机的服务进程
>
> + 数据库存储用户信息，支持用户注册找回密码，预计支持**邮件**找回密码
> + 文件传输改为TCP，采用多线程传输
> + 支持好友机制，支持图片发送
> + 离线消息存入数据库，读取数据库

