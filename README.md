# Wikjxwrt-snapshots 云编译固件

固件已加入OTA在线更新（固件编译显示时间为UTC），目前只支持镜像为wikjxwrt-x86-64-generic-ext4-combined-efi.img.gz安装的版本其他版本暂时不要尝试在线升级功能后续会继续适配。

### 本固件源码基于openwrt-snapshots修改，云编译项目。
   本仓库为Wikjxwrt的github云编译库，与一键编译脚本所产出固件一致。
   
   官方源码仓库 - [OpenWrt-24.10](https://github.com/openwrt/openwrt/tree/openwrt)
   
   本固件源码仓库 - [OpenWrt-24.10](https://github.com/wixxm/OpenWrt-snapshots)

#### 固件下载地址
   - [Github](https://github.com/wixxm/wikjxwrt-snapshots/releases)
  
   - [Google](https://drive.google.com/drive/folders/1ORaVqeKyvWItATbq0NCFNysLSOhb6Q2N?usp=sharing)
### 固件说明
#### 支持硬件 
- [x] X86_64

#### 登录信息
```
地址：192.168.88.1（修改代码：vi /etc/config/network）
用户：root
密码：空
```
---------------

#### 附加功能
 SSH中添加固件信息的显示
 |  信息 | 参数  | 
 |  :----  |  :----  |
 | 系统负载:   0.00 0.06 0.03 | 运行时间:   0 days   | 
 | 内存已用:   7% of 3936MB  |  交换内存:   0% of 0MB   | 
 | CoreMark:   58293.635974 | 存储使用:   39% of 990.7M |
 |IP地址:     192.168.88.1 | CPU 型号:  | 
  
添加了首次安装固件之后的第二天自动进行coremark测试并且显示到SSH登录信息
也可以通过手动运行  /etc/coremark.sh 进行coremark测试同时也会显示在SSH信息中
   
   
   
#### 集成插件
 |  服务 | 系统  |  网络  |
  |  :----  |  :----  |  :----  |
  | passwall | netdata | iperf3 |
  |微信推送 | CPU Load | UPnP |
  | MosDNS | Argon config | Turbo ACC 网络加速设置 |
  | openwrtclash | DiskMan | BBR |
  | lucky | statistics | nlbwmon |
  | nikki | | MultiWAN 管理器 |
  | 宽带监控 | | |
  | 网络共享 | | |
  | 终端 | | |
  | MWAN3 分流助手 | | | 
 

### 本地编译
   如需本地编译固件可直接使用本固件一键编译脚本即可编译出完全相同固件
   - [WikjxWrt-Auto](https://github.com/wixxm/wikjxwrt-auto)
