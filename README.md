#0.前置准备

apt-get update & apt-get install -y xz-utils openssl gawk file

or

apt update & apt install -y xz-utils openssl gawk file


#1.Ubuntu 20.04 / Debian 12 一键DD

bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/CarrolChen/VPS_DD_Script/master/install.sh') -u 20.04 -v 64 -p you_set_password -port 22 -a -firmware

or

bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/CarrolChen/VPS_DD_Script/master/install.sh') -d 12 -v 64 -p you_set_password -port 22 -a -firmware


#2.SSH连接

user：root

port：22

password：you_set_password
