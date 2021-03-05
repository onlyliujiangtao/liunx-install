下载安装包
```
wget http://mirrors.cnnic.cn/apache/tomcat/tomcat-8/v8.0.24/bin/apache-tomcat-8.0.24.tar.gz
```
解压安装包
```
tar xf apache-tomcat-8.0.24.tar.gz -C /usr/local/
```
安装
```
cd /usr/local/
ln -sv apache-tomcat-8.0.24 tomcat
```
配置环境变量：
```
vim /etc/profile
```
```js
//写入
CATALINA_BASE=/usr/local/tomcat
PATH=$CATALINA_BASE/bin:$PATH
export PATH CATALINA_BASE
```
```js
//重读此文件，让变量生效
. /etc/profile
```
.查看tomcat版本状态
```
catalina.sh version
```
配置server.xml