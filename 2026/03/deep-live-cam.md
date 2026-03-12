# Deep-Live-Cam 本地安装指南

## 视频中共享的安装包

- <a href="https://pan.baidu.com/s/1yc3rgo_5bMU8fLVGNWUzEA?pwd=rwc1" target="_blank">百度网盘</a>
- [谷歌网盘](https://drive.google.com/drive/folders/1QooadBVwXfpRwxTrEwYmuUDSB4DWzegG?usp=drive_link)  

---

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

---

## 四、安装依赖包

```bash
# 创建虚拟环境
python -m venv venv

# 激活虚拟环境 (Windows)
call venv\scripts\activate

# 安装依赖
pip install -r requirements.txt
