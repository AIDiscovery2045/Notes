# Deep-Live-Cam 本地安装

## 一、检查更新显卡驱动

确保英伟达显卡驱动版本 ≥ 525。

---

## 二、安装 CUDA 与 cuDNN

- **CUDA 12.8**  
  下载链接: [CUDA 12.8 下载](https://developer.nvidia.com/cuda-12-8-0-download-archive)  

- **cuDNN 8.9**  
  下载链接: [cuDNN 8.9 下载](https://developer.nvidia.com/rdp/cudnn-archive)  

---

## 三、安装相关依赖程序

1. **FFmpeg**（版本 ≥ 6.0）  
2. **Visual Studio 工具**  
3. **Python 3.11**  
4. **Git 工具**  
5. **下载 Deep-Live-Cam**

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
