# Sing-box 多协议一键部署脚本

一个 Sing-box 自动化部署工具，支持多协议自选部署和线路机中转的完整解决方案。

本项目基于 [caigouzi121380/singbox-deploy](https://github.com/caigouzi121380/singbox-deploy) 修改而来。

原项目地址：https://github.com/caigouzi121380/singbox-deploy

---
## 一键部署命令

安装全功能 sing-box：

```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/caigouzi121380/singbox-deploy/main/install-singbox-yyds.sh)"
```

## 主要特性

- **多系统支持** - 支持 Alpine, Debian, Ubuntu, CentOS, RHEL, Fedora 等操作系统
- **管理工具** - 输入 sb 指令进入管理界面查看节点链接、重置端口、服务端控制查看等功能
- **开机自启** - 自动配置 Systemd / OpenRC 开机自启，崩溃自动拉起服务端
- **灵活端口** - 支持自动寻找空闲端口或手动指定

### 部署机功能

- **一键安装** - 自动部署 Sing-box 最新服务端
- **自动生成** - 自动生成 密钥和配置文件，VLESS Reality 自选或默认SNI
- **连接 IP** - 自动获取公网 IP 或手动输入 连接IP/DDNS域名 并生成客户端链接

### 线路机功能

- **一键生成** - 从落地机直接生成线路机安装脚本
- **一键出站** - 可直接添加落地机链接来添加出站
- **多路入站** - 可生成多个入站来配合出站
- **流量转发** - 自动转发流量到落地机节点
