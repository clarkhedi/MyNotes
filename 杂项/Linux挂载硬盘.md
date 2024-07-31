
## 具体步骤

### 1、查看硬盘挂载情况

```
sudo fdisk -l    // 根据硬盘大小可以知哪块硬盘没挂载， 比如 /dev/sdb
```

### 2、查看当前分区情况

```
df -l
```

### 3、给新硬盘添加新分区

```
sudo fdisk /dev/sdb
```
按照下面步骤依次输入指令


sudo blkid           // 可以找到sda的UUID
//挂载配置，比如挂载到 /sdb 这个目录，若没有可以 mkdir /sdb
sudo vim /etc/fstab



