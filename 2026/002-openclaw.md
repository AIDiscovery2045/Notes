# OpenClaw安全部署与彻底卸载教程

## 1、下载安装Node.js

Node.js版本 ≥ 22 [下载链接](https://nodejs.org/en/download)

---

## 2、下载安装Git工具
Git官网下载最新安装程序  [下载链接](https://git-scm.com/install/windows)

---

## 三、安装OpenClaw

1. 搜索PowerShell，以管理员身份运行
2. 安装前依次执行以下指令，检查设置系统环境
```
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```
```
netstat -ano | findstr 18789
```
```
taskkill /PID 最后一列ID /F
```


4. **Python 3.11**  
5. **Git 工具**  
6. **下载 Deep-Live-Cam**

### ( 附共享的安装包下载)
- 百度网盘: <a href="https://pan.baidu.com/s/1yc3rgo_5bMU8fLVGNWUzEA?pwd=rwc1" target="_blank">点击下载</a>  
- 谷歌网盘: <a href="https://drive.google.com/drive/folders/1QooadBVwXfpRwxTrEwYmuUDSB4DWzegG?usp=drive_link" target="_blank">点击下载</a>  
---

## 四、安装依赖包
1、**创建虚拟环境**
```bash
python -m venv venv
```
2、**激活虚拟环境**
```bash
call venv\scripts\activate
```
3、**安装依赖包**
```bash
pip install -r requirements.txt
```

