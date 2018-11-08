# 20181108 Ubuntu 登录ssh鉴权未通(密码正确）

securecrt正常输入帐号密码，登录反映鉴权失败

1. 重新安装 

   ```
   sudo apt-get install openssh-server
   
   ```

2. 查看进程

   ```
   ps -e | grep ssh
   ```

   ![](img\QQ截图20181108151201.png)

3. 查看状态

   ```
   /etc/init.d/ssh status
   ```

   ![](img\QQ截图20181108151526.png)

4. 重新securecrt连接成功

   （可能开始了新的ssh服务）