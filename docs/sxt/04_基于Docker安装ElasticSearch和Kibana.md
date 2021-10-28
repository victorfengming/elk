# 04_基于Docker安装ElasticSearch和Kibana.

> created by victorfengming

安装 ES6.x要求linux的内核版本是3.5+版本以上

然后我们校验linux 版本的方式就是

```shell
[root@iz8g9301trfnpxz ~]# uname -a
Linux iz8g9301trfnpxz 3.10.0-1127.19.1.el7.x86_64 #1 SMP Tue Aug 25 17:23:54 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux
[root@iz8g9301trfnpxz ~]#
```

## 1. 为elasticsearch提供完善的系统配置

es在linux中安装部署的时候,需要系统为其提供若干系统配置.

如: 应用可启动线程数,应用可以在系统中划分的虚拟内存,应用可以最多创建多少个文件等.

### 修改限制信息

是修改系统中允许应用最多创建多少个文件等的限制权限

> linux默认来说,一般限制应用最多创建的文件是65535个.
>
> 但是elasticsearch至少需要65535的文件创建权限.



修改如下:

```shell
vim /etc/securitylimits.conf
```

```
[root@iz8g9301trfnpxz ELK]# cat /etc/securitylimits.conf
* soft nofile 65536
* hard nofile 65536

[root@iz8g9301trfnpxz ELK]# 
```

### 修改线程数量限制

```shell
[root@iz8g9301trfnpxz ELK]# cat /etc/securitylimits.conf
*       soft nofile 65536
*       hard nofile 65536
*       soft nproc 4096
root    soft nproc unlimited
[root@iz8g9301trfnpxz ELK]# 
```

`4096*250k = 1.5G`,要求你虚拟机内存至少要1.5GB,推荐提供内存2G+

unlimited 这个只能用在 root用户,不可设置到其他用户!!!**敲黑板


### 修改系统

