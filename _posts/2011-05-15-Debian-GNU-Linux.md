---
layout: post
title: Debian GNU/Linux 使用技巧
---

# 1. 使用 Jigdo 下载 Debian 系统镜像文件

[Jigdo](http://atterer.org/jigdo/) 是一个系统镜像文件下载工具，它可以利用已有的 Debian GNU/Linux 镜像文件，从而为你节省网络流量。

1. 安装 `jigdo-file`：`sudo apt install jigdo-file`
2. 如果有已经下载好的镜像文件，将其挂载到 `/mnt` 相应路径下
2. 使用 `jigdo-lite` 命令，提供 jigdo 文件或文件网址、本地解压后的镜像文件路径（用于扫描）、待下载的镜像地址（非镜像文件，而是**镜像文件包**的地址，如https://mirrors.ustc.edu.cn/debian-cdimage/weekly-builds/amd64/jigdo-dlbd/）

```bash
# cd /data/debian-testing-dlbd
# mount debian-testing-amd64-DLBD-1.iso /mnt/dlbd1
# mount debian-testing-amd64-DLBD-2.iso /mnt/dlbd2
# rm -rf 1 2 && mkdir -pv 1 2
# # 分别进入 1、2 两个临时目录执行 jigdo-lite 命令（亦可不用手动执行 wget 命令，jigdo-lite 会自动下载 template 文件）
# cd 1
# wget -c "https://mirrors.ustc.edu.cn/debian-cdimage/weekly-builds/amd64/jigdo-dlbd/debian-testing-amd64-DLBD-1.template"
# jigdo-lite "https://mirrors.ustc.edu.cn/debian-cdimage/weekly-builds/amd64/jigdo-dlbd/debian-testing-amd64-DLBD-1.jigdo"
# 
You can also enter a single digit from the list below to
select the respective entry for scanning:
  1: /mnt/dlbd2/
  2: /mnt/dlbd1/
Files to scan: 2

```

# 2. 使用 `apt-cdrom` 设置镜像源

# 3. 配置 sudo 免密码，控制台 root 免密码登录
