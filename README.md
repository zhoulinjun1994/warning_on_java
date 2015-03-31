# warning_on_java
一个在Ubuntu服务器上配置java和tomcat的问题：
Ubuntu系统自带一个openjdk的jdk版本，但是这个版本功能弱爆了~
所以呢~
要下载jdk后切换一下工作中的jdk，命令为：
sudo update-alternatives --install /usr/bin/java java /opt/jdk1.7.0_17/bin/java 300
sudo update-alternatives --config java
这样就可以选择自己版本的jdk了

如果用openjdk，会出现一些问题，比如tomcat无法加载静态资源等（找不到工作目录）
