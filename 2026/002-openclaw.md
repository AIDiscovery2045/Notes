# OpenClaw安全部署与彻底卸载教程

## 1、下载安装Node.js

Node.js版本 ≥ 22 [下载链接](https://nodejs.org/en/download)

检查Node.js是否成功安装
```
node --v
```
检查npm是否成功安装
```
npm --version
```
---

## 2、下载安装Git工具
Git官网下载最新安装程序  [下载链接](https://git-scm.com/install/windows)

检查Git是否成功安装
```
git --version
```

---

## 三、安装OpenClaw

1. **系统开始菜单->搜索PowerShell，以管理员身份运行**
2. **安装前依次执行以下指令，检查、设置系统环境**

开启允许脚本执行策略
```
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```
国内用户，推荐设置npm镜像地址
```
npm config set registry  https://registry.npmmirror.com
```
(恢复npm官方地址)
```
npm config set registry https://registry.npmjs.org
```
检查18789端口是否被占用
```
netstat -ano | findstr 18789
```
如果18789端口被占用，强制释放端口
```
taskkill /PID 最后一列ID /F
```

3.**安装OpenClaw**
```
iwr -useb https://openclaw.ai/install.ps1 | iex
```
---

## 四、运行配置向导
```
openclaw onboard --install-daemon
```

**第1步：选择工作区路径**
 OpenClaw的数据（配置文件、聊天记录、技能等）存在哪个目录，推荐默认(回车）
**第2步：选择AI模型提供商**
 选择OpenClaw接入哪个服务商的大模型
**第3步：输入接入模型的API Key**

**第4步：配置网关端口** 
默认是18789（回车)
**第5步：通信通道配置** 
可选"跳过(skip)"
**第6步：是否安装守护进程**
是否安装守护进程，是（Y）
**第7步：确认配置摘要**
回车确认

## 五、首次运行
PowerShell里运行指令
```
openclaw gateway --port 18789
```
可以新开一个PowerShell窗口查看是否运行
```
openclaw gateway status
```
如果安装了守护进程，电脑重启后可以直接在浏览器打开OpenClaw
http://127.0.0.1:18789/


---



