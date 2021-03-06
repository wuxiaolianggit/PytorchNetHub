# 本仓库目的

- 如果不想阅读源码，推荐看原仓库地址，感谢大佬们的无私奉献！
- 本仓库将代码改为统一风格，能够更容易、更轻松得阅读源码，以便根据自己需求进行修改。

# 接下来工作

### 目标检测
- [x] Faster rcnn
- [x] YOLO v1
- [x] YOLO v3
- [x] SSD
- [x] CAM
- [x] S4ND
- [x] YOLO v4

### 语义分割
- [x] U-Net

### 其他
- [x] SKNet
- [x] FPN特征金字塔网络
- [x] Noise2noise
- [x] FunnelAct
- [ ] Circle-Loss
- [ ] 该仓库将拆分为多个子仓库，仅保留readme.md



# 汇总

|模型|原仓库|加注释|实现|来源|备注|更新|
|:---:|:----:|:---:|:------:|:------:|:------:|:------:|
|[Fatser Rcnn](https://arxiv.org/abs/1506.01497) |[原地址](https://zhuanlan.zhihu.com/p/32404424)|[注释](https://github.com/bobo0810/PytorchNetHub/tree/master/FasterRcnn_pytorch)||NIPS 2015||
|[YOLO v1](https://arxiv.org/abs/1506.02640) |[原地址](https://github.com/xiongzihua/pytorch-YOLO-v1)|[注释](https://github.com/bobo0810/AnnotatedNetworkModelGit/tree/master/Yolov1_pytorch)||CVPR2016||
|[YOLO v3](https://pjreddie.com/media/files/papers/YOLOv3.pdf) |[原地址](https://github.com/eriklindernoren/PyTorch-YOLOv3)|[注释](https://github.com/bobo0810/PyTorch-YOLOv3-master)|[重构](https://github.com/bobo0810/AnnotatedNetworkModelGit/tree/master/Yolov3_pytorch)|||
|[YOLO v4](https://arxiv.org/pdf/2004.10934.pdf) |[原地址](https://github.com/Tianxiaomo/pytorch-YOLOv4)|[注释](https://github.com/bobo0810/YOLOv4_Pytorch)||||2020.4|
|[SSD](https://arxiv.org/abs/1512.02325)|[原地址](https://github.com/amdegroot/ssd.pytorch)|[注释](https://github.com/bobo0810/pytorchSSD)|[重构](https://github.com/bobo0810/AnnotatedNetworkModelGit/tree/master/SSD_pytorch)|ECCV2016||
|[CAM](https://arxiv.org/pdf/1512.04150.pdf) |[原地址](https://github.com/jacobgil/keras-cam)|[注释](https://github.com/bobo0810/AnnotatedNetworkModelGit/tree/master/CAM_pytorch)||CVPR2016|卷积层实现弱监督定位|
|[S4ND](https://arxiv.org/pdf/1805.02279.pdf?fbclid=IwAR0B3dI8tjvWz-Mk9Xpyymfnk-SNs6k8tw2B8HU3dTTP-vFinQURHGZSCQs) |||[复现](https://github.com/bobo0810/S4ND_Pytorch)|MICCAI 2018|单次单尺度肺结节检测|
|[U-Net](https://arxiv.org/abs/1505.04597)|[原地址](https://github.com/milesial/Pytorch-UNet)|[注释](https://github.com/bobo0810/AnnotatedNetworkModelGit/tree/master/UNet_pytorch) ||MICCAI2015||
|[SKNet]((https://arxiv.org/abs/1903.06586))|[原地址](https://github.com/implus/SKNet)||[实现](https://github.com/bobo0810/SKNet_Pytorch)|CVPR2019|继Res\Dense\SE之后新型Block|2019.5|
|[Noise2noise](https://arxiv.org/abs/1803.04189)|[原地址](https://github.com/joeylitalien/noise2noise-pytorch)||[重构](https://github.com/bobo0810/AnnotatedNetworkModelGit/tree/master/Noise2noise_pytorch)|ICML2018||
|[FPN](https://arxiv.org/abs/1612.03144)|[原地址](https://github.com/kuangliu/pytorch-fpn)|[注释](https://github.com/bobo0810/AnnotatedNetworkModelGit/tree/master/FPN_pytorch)||CVPR2017||
|[FunnelRelu](https://arxiv.org/pdf/2007.11824.pdf)|[原地址](https://github.com/megvii-model/FunnelAct) ||[复现](https://github.com/bobo0810/FunnelAct_Pytorch)||较Relu\PRelu\Swish更有效|2020.7|


注：猫狗大战、风格迁移、GAN生成对抗网络等更多内容请访问[传送门](https://github.com/chenyuntc/pytorch-book)

# 阅读源码三步骤

- 数据预处理
- 网络模型搭建
- 损失函数定义

# 项目一般结构


- 总结构

  ![](https://github.com/bobo0810/imageRepo/blob/master/img/99053959.jpg)
  
  
- 项目结构

  1、定义网络
  
  ![](https://github.com/bobo0810/imageRepo/blob/master/img/16409622.jpg) 
  
   2、封装数据集
   
  ![](https://github.com/bobo0810/imageRepo/blob/master/img/38894621.jpg)
  
   3、工具类
   
  ![](https://github.com/bobo0810/imageRepo/blob/master/img/98583532.jpg)
  
   4、主函数
   
  ![](https://github.com/bobo0810/imageRepo/blob/master/img/32257225.jpg)

