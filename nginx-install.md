下载
wget http://nginx.org/download/nginx-1.9.9.tar.gz

解压
tar -xzvf nginx-1.9.9.tar.gz


进入nginx-1.9.9

运行./configure

如果没有gcc
安装  yum install -y gcc
如果没有PCRE
安装 yum install -y pcre-devel
如果没有zlib
安装 yum install -y zlib-devel

编译

make install


进入 /sur/local/nginx


cd /usr/local/nginx/sbin

　　启动：./nginx
　　停止：./nginx -s stop
　　重启：./nginx -s reopen
　　执行./nginx -h 可以看到命令的帮助信息
<!-- 建立软连接全局访问 -->
ln -s /usr/local/nginx/sbin/nginx /usr/local/sbin/
