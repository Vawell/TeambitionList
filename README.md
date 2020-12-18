# TeambitionList
测试站点如下

https://teambition.icu/

测试直链如下

https://teambition.icu/file/5fb299670da0d8497bb5be74/447dfc3af4283d63812271e27878ca4e/js.mp4

安装方法如下


linux服务器：


依次执行如下命令

wget https://one.blob.core.chinacloudapi.cn/badyun/teambition/v0.01/app
chmod +x ./app
./app



然后在宝塔后台添加反向代{过}{滤}理即可





进程守护可以使用nohup或者pm2


nohup方式命令为：
nohup ./app &


输入完成后连按两下回车

pm2方式需要先到宝塔后台软件管理安装pm2管理器

然后登录服务器进到程序目录执行
[Bash shell] 纯文本查看 复制代码
pm2 start app --name teambition
pm2 save
pm2 startup

关闭程序的话，执行下面的命令
#获取pid
sudo lsof -i:5213
  
#结束进程
sudo kill -9 你上面查到的pid


win服务器：


直接下载如下链接运行即可


https://one.blob.core.chinacloudapi.cn/badyun/teambition/v0.01/app.exe


