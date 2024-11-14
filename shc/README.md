### 编译安装SHC

```shell
[root@localhost ~]# cd /opt/soft/
[root@localhost soft]# wget http://www.datsi.fi.upm.es/~frosal/sources/shc-3.8.9b.tgz
[root@localhost soft]# tar xvf shc-3.8.9b.tgz
[root@localhost soft]# cd shc-3.8.9b/
 
# 创建目录这一步这个是必须的，没这个目录会报错
[root@localhost shc-3.8.9b]# mkdir -p /usr/local/man/man1/
[root@localhost shc-3.8.9b]# make install 
```

### 使用SHC加密脚本
- 脚本开头必须有魔法字符，例如 `!/usr/bin/bash`
```bash
[root@localhost shc-3.8.9b]# shc -v -r -T -f /script/script.sh
```
