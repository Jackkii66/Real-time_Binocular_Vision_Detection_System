# Real-time_Binocular_Vision_Detection_System 
# 基于深度学习的实时双目视觉检测系统
2019/11/05      
小组成员：Jackkii, ...

#### 简介
*使用动态权衡时效和精度的实时深度估计算法，搭配轻量卷积神经网络，为算力有限的平台提供深度估计与目标检测功能。*

#### 详细介绍

#### 环境依赖 ?
* python3
* pytorch
* linux
* Jetson Nano
* 小觅双目相机


#### 目录结构描述 ?
├── Readme.md                       
├──                                
├──         



#### 版本更新 ?
######V1.0.0 基本功能实现      
2019/11/

1.     
2.

#### AnyNet-master/together.py —— 2020/2/29
1、安装了skimage包，安装过程如下：
```
sudo pip3 install --upgrade setuptools
sudo pip3 install scikit-image -i http://pypi.douban.com/simple/ --trusted-host pypi.douban.com
```
2、cuda没问题，但cudnn有异常，
按照：[参考文章](https://blog.csdn.net/Ocean_waver/article/details/102730467)
最后一句运行有错，显示cudnn冲突，似乎pytorch安装之后cudnn有过改动，anynet是否可用还有待验证。

3、考虑下载使用anynet部分新代码，以适配 jetson nano 上的 pytorch1.0 和 cuda10。
