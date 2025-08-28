```bash
#0.前置准备
apt-get update & apt-get install -y xz-utils openssl gawk file
or
apt update & apt install -y xz-utils openssl gawk file


#1.Ubuntu 20.04 / Debian 12 一键DD
bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/CarrolChen/VPS_Script/master/install.sh') -u 20.04 -v 64 -p you_set_password -port 22 -a -firmware
or
bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/CarrolChen/VPS_Script/master/install.sh') -d 12 -v 64 -p you_set_password -port 22 -a -firmware


#2.SSH连接
user：root
port：22
password：you_set_password


#3.docker一键安装
chmod -R 777 /root/docker_install.sh
source docker_install.sh

#4.nezha探针部署（D:V0.20.13,A:V0.20.5）
chmod -R 777 /root/nezha_install.sh
source nezha_install.sh

#5.nezha主题前端UI美化（docker方式安装）
a.将template里面的文件放到服务器路径：/opt/nezha/dashboard/theme-custom/template里面
b.docker ps
c.docker restart 上一步中哪吒的id
d.登录哪吒面板后台，设置===>主题==>选择Custom(local)
e.将css.txt里面的CSS样式代码复制到哪吒面板后台的“自定义代码”文本框里，保存即可
```
