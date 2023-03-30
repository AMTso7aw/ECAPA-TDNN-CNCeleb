# 介绍
这个项目基于 [ECAPA-TDNN](https://github.com/TaoRuijie/ECAPA-TDNN) 所修改。

## 性能
> 还在测试中，见谅。

# Quick Start

## 准备工作
此项目针对 [CN-Celeb](http://cnceleb.org/) 数据集进行训练测试。

### 数据
* CN-Celeb 1  [[点此下载]](http://openslr.org/82/)
* CN-Celeb 2  [[点此下载]](http://openslr.org/82/)
> CN-Celeb 原始数据是 flac 格式，考虑到转换格式又要占磁盘空间，就直接读取 flac 格式进行训练了。

### 环境

```
conda create -n cnceleb python=3.8.13 anaconda
conda activate cnceleb
pip install -r requirements.txt -i https://pypi.mirrors.ustc.edu.cn/simple/
```
> pip 安装不了可以试试下面其他的源
> * 清华：https://pypi.tuna.tsinghua.edu.cn/simple/
> * 阿里云：http://mirrors.aliyun.com/pypi/simple/
> * 中国科技大学 https://pypi.mirrors.ustc.edu.cn/simple/
> * 华中理工大学：http://pypi.hustunique.com/
> * 山东理工大学：http://pypi.sdutlinux.org/
> * 豆瓣：http://pypi.douban.com/simple/


## 训练
1. 在 `trainECAPAModel.py` 配置好对应路径
2. 激活 conda 环境 `conda activate cnceleb`
3. 运行 `python trainECAPAModel.py`

## 测试
运行`python trainECAPAModel.py --eval`

## Acknowledge

参考了以下这些项目，感谢各位前辈！

[TaoRuijie/ECAPA-TDNN](https://github.com/TaoRuijie/ECAPA-TDNN)

[Lantian Li/Sunine](https://gitlab.com/csltstu/sunine)
