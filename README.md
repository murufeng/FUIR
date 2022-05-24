[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/simple-baselines-for-image-restoration/image-deblurring-on-gopro)](https://paperswithcode.com/sota/image-deblurring-on-gopro?p=simple-baselines-for-image-restoration)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/simple-baselines-for-image-restoration/image-denoising-on-sidd)](https://paperswithcode.com/sota/image-denoising-on-sidd?p=simple-baselines-for-image-restoration)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/maxim-multi-axis-mlp-for-image-processing/deblurring-on-hide-trained-on-gopro)](https://paperswithcode.com/sota/deblurring-on-hide-trained-on-gopro?p=maxim-multi-axis-mlp-for-image-processing)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/vrt-a-video-restoration-transformer/deblurring-on-reds)](https://paperswithcode.com/sota/deblurring-on-reds?p=vrt-a-video-restoration-transformer)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/restormer-efficient-transformer-for-high/single-image-deraining-on-rain100h)](https://paperswithcode.com/sota/single-image-deraining-on-rain100h?p=restormer-efficient-transformer-for-high)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/restormer-efficient-transformer-for-high/single-image-deraining-on-rain100l)](https://paperswithcode.com/sota/single-image-deraining-on-rain100l?p=restormer-efficient-transformer-for-high)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/restormer-efficient-transformer-for-high/single-image-deraining-on-test100)](https://paperswithcode.com/sota/single-image-deraining-on-test100?p=restormer-efficient-transformer-for-high)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/restormer-efficient-transformer-for-high/single-image-deraining-on-test1200)](https://paperswithcode.com/sota/single-image-deraining-on-test1200?p=restormer-efficient-transformer-for-high)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/restormer-efficient-transformer-for-high/single-image-deraining-on-test2800)](https://paperswithcode.com/sota/single-image-deraining-on-test2800?p=restormer-efficient-transformer-for-high)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/nafssr-stereo-image-super-resolution-using/stereo-image-super-resolution-on-flickr1024-1)](https://paperswithcode.com/sota/stereo-image-super-resolution-on-flickr1024-1?p=nafssr-stereo-image-super-resolution-using)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/nafssr-stereo-image-super-resolution-using/stereo-image-super-resolution-on-flickr1024-2)](https://paperswithcode.com/sota/stereo-image-super-resolution-on-flickr1024-2?p=nafssr-stereo-image-super-resolution-using)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/nafssr-stereo-image-super-resolution-using/stereo-image-super-resolution-on-kitti2012-2x-1)](https://paperswithcode.com/sota/stereo-image-super-resolution-on-kitti2012-2x-1?p=nafssr-stereo-image-super-resolution-using)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/nafssr-stereo-image-super-resolution-using/stereo-image-super-resolution-on-kitti2012-4x)](https://paperswithcode.com/sota/stereo-image-super-resolution-on-kitti2012-4x?p=nafssr-stereo-image-super-resolution-using)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/nafssr-stereo-image-super-resolution-using/stereo-image-super-resolution-on-kitti2015-2x)](https://paperswithcode.com/sota/stereo-image-super-resolution-on-kitti2015-2x?p=nafssr-stereo-image-super-resolution-using)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/nafssr-stereo-image-super-resolution-using/stereo-image-super-resolution-on-kitti2015-4x)](https://paperswithcode.com/sota/stereo-image-super-resolution-on-kitti2015-4x?p=nafssr-stereo-image-super-resolution-using)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/nafssr-stereo-image-super-resolution-using/stereo-image-super-resolution-on-middlebury-1)](https://paperswithcode.com/sota/stereo-image-super-resolution-on-middlebury-1?p=nafssr-stereo-image-super-resolution-using)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/nafssr-stereo-image-super-resolution-using/stereo-image-super-resolution-on-middlebury)](https://paperswithcode.com/sota/stereo-image-super-resolution-on-middlebury?p=nafssr-stereo-image-super-resolution-using)

# A Flexible and Unified Image Restoration Framework. 

[![GitHub stars](https://img.shields.io/github/stars/murufeng/FUIR.svg?style=social&label=Stars)](https://github.com/murufeng/FUIR)
[![GitHub forks](https://img.shields.io/github/forks/murufeng/FUIR.svg?style=social&label=Forks)](https://github.com/murufeng/FUIR)
[![download](https://img.shields.io/github/downloads/murufeng/FUIR/total.svg)](https://github.com/murufeng/FUIR/releases) 
![visitors](https://visitor-badge.glitch.me/badge?page_id=murufeng/FUIR)

> 当前，对于Low-level-Vision中的图像恢复任务（Image Super-resolution, Image Denoising, Image Deblurring等) 已经出现了很多优秀实用的工具包。 
>但是，对于去年出现的一系列Transformer网络架构还没有一个统一的项目将它集成起来，本项目主要在具体图像恢复任务的数据处理和网络训练配置上将当前主流的CNN网络和基于Transformer的网络架构集成了起来。本项目将作为图像恢复任务的一个灵活统一的工具。利用本项目可以快速实现图像去噪，图像/视频去模糊，图像去雨等一系列经典任务的训练。 
>本项目提供在GOPRO、SIDD、REDS、Rain13K数据集上的数据预处理以及网络架构训练教程，后续我们将持续更新。希望本项目既能让图像处理初学者快速入门，又能服务科研和工业社区。

### Installation

See [INSTALL.md](https://github.com/murufeng/FUIR/blob/main/INSTALL.md) for the installation of dependencies required to run FUIR.


### News
 * *2022-5-17* Update the State-of-the-Art models, such as NAFNet, Restormer, MPRNet, HINet, MIMO-UNet

### Model Zoo

<details>
<summary>NAFNet</summary> 
网络模块结构如下所示：

![](./figures/NAFNet_block.jpg)

模块设计如下：

![](./figures/nafnet_fig_1.jpg)

两大经典图像恢复实验结果如下：
1. Image Denoising （在SIDD数据集实现SOTA):

![](./figures/nafnet_tab_1.jpg)

2. Image Deblurring （在GoPro数据集实现SOTA):

![](./figures/nafnet_tab_2.jpg)

[模型训练配置](./docs)

[模型训练代码](./options/train)

</details>

<details>
<summary>Restormer</summary> 

网络模块结构如下所示：
![](./figures/restormer_block.jpg)

三大图像恢复实验结果对比图：
![](./figures/restormer_fig_1.jpg)

1. Image Deraining(目前保持SOTA):

![](./figures/restormer_tab_1.jpg)
![](./figures/restormer_vis_1.jpg)

2. Image Deblurring:

![](./figures/restormer_tab_2.jpg)

3. Image Denoising:

![](./figures/restormer_tab_3.jpg)

[模型训练配置](./docs)

[模型训练代码](./options/train)

</details>

<details>
<summary>HINet</summary> 

网络模块结构如下所示：
![](./figures/HINet.jpg)
![](./figures/HINet_block.jpg)

#### 三大图像恢复实验结果：
1. Image Denoising:

![](./figures/hinet_tab_1.jpg)

2. Image Deblurring:

![](./figures/hinet_tab_2.jpg)

3. Image Deraining:

![](./figures/hinet_tab_3.jpg)

[模型训练配置](./docs)

[模型训练代码](./options/train)

</details>

<details>
<summary>MPRNet</summary> 

网络模块结构如下所示：
![](./figures/mprnet.jpg)

#### 三大图像恢复实验结果：

1. Image Deraining:
![](./figures/mprnet_tab_1.jpg)
![](./figures/mprnet_derain.jpg)
2. Image Deblurring:
![](./figures/mprnet_tab_2.jpg)
3. Image Denoising:
![](./figures/mprnet_tab_3.jpg)

[模型训练配置](./docs)

[模型训练代码](./options/train)

</details>


<details>
<summary>MIMONet</summary> 

网络模块结构如下所示：

![](./figures/mimo_unet.jpg)

图像去模糊实验结果与可视化图：

![](./figures/mimo_unet_tab_1.jpg)

![](./figures/mimo_unet_fig_1.jpg)

</details>

<details>
<summary>MIRNet</summary> 

网络模块结构如下所示：
![](./figures/mirnet_network.jpg)

![](./figures/mirnet_att.jpg)

![](./figures/mirnet_skff.jpg)
</details>

<details>
<summary>SCUNet</summary> 

网络模块结构如下所示：

![](./figures/SCUNet.jpg)

部分实验结果如下：
![](./figures/scunet_tab_2.jpg)

![](./figures/SCUNet_vis.jpg)

![](./figures/scunet_vis_2.jpg)

</details>


### Experiments 

### Image Restoration Tasks 

| Task                                 | Dataset | Train/Test Instructions                                                
| :----------------------------------- | :------ | :---------------------- | 
| Image Deblurring                     | GoPro   | [link](./docs/GoPro.md) | 
| Image Denoising                      | SIDD    | [link](./docs/SIDD.md)  | 
| Image Deblurring with JPEG artifacts | REDS    | [link](./docs/REDS.md)  | 
| Image Derain                         | Rain13K    | [link](./docs/Rain.md)  |
| Stereo Image Super-Resolution | Flickr1024+Middlebury    | [link](./docs/StereoSR.md) 

### Citations
If you find this project is useful, please give me a star and fork!

### Contact

If you have any questions, please contact me. 2394849504@qq.com

---

## Acknowledgment

This implementation based on [BasicSR](https://github.com/xinntao/BasicSR) and [NAFNet](https://github.com/megvii-model/NAFNet).


<details>
<summary>statistics</summary> 

![visitors](https://visitor-badge.glitch.me/badge?page_id=murufeng/FUIR)

</details>
