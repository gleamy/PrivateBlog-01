## cent os 常用命令
### 系统信息命令
```sh
grep "model name" /proc/cpuinfo # 查看CPU信息
grep MemTotal /proc/meminfo # 查看内存总量

# 其实可以通过如下命令查看全部信息
cat /proc/cpuinfo
cat /proc/meminfo

uname -a  # 查看操作系统信息
getconf LONG_BIT # 可以查看操作系统是 32 位还是64位。
```
### 查看容量
```sbtshell
df -h # 查看系统磁盘使用情况， -h 总计为大单位；
du -h --max-depth=1 /home # 查看某目录的容量， -h 同上， --max-depth 用来指定深入目录的层数，为1就指定1层
```