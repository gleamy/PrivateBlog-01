## JAVA 环境配置：
- 检查： 通过 java -version 命令检查系统是否已经安排 java 环境。<br />
另一种方式：yum list installed |grep java。
- 检查：如果操作系统不是最小安装，会默认安装openjdk，可以通过如下命令检查环境中是否存在 openjdk. <br />
\# rpm -qa | grep java <br />
假如存在，可以通过下面的命令进行删除。<br />
 \# rpm -e --nodeps `rpm -qa | grep java` , 另一种方式 yum -y remove java-1.7.0-openjdk*
 
- 下载：<br />
wget http://download.oracle.com/otn-pub/java/jdk/8u151-b12/e758a0de34e24606bca991d704f6dcbf/jdk-8u151-linux-x64.tar.gz
    > 经测试，之上的方法文件下载不全， 最后只能在本地下载并上传。

- 解压：# tar -zxvf jdk-8u151-linux-x64.tar.gz 
- 配置环境变量


