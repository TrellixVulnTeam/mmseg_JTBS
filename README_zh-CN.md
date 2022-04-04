<div align="center">
  <img src="resources/mmseg-logo.png" width="600"/>
  <div> </div>
  <div align="center">
    <b><font size="5">OpenMMLab 官网</font></b>
    <sup>
      <a href="https://openmmlab.com">
        <i><font size="4">HOT</font></i>
      </a>
    </sup>
        
    <b><font size="5">OpenMMLab 开放平台</font></b>
    <sup>
      <a href="https://platform.openmmlab.com">
        <i><font size="4">TRY IT OUT</font></i>
      </a>
    </sup>
  </div>
  <div> </div>
</div>
<br />

[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mmsegmentation)](https://pypi.org/project/mmsegmentation/)
[![PyPI](https://img.shields.io/pypi/v/mmsegmentation)](https://pypi.org/project/mmsegmentation)
[![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmsegmentation.readthedocs.io/zh_CN/latest/)
[![badge](https://github.com/open-mmlab/mmsegmentation/workflows/build/badge.svg)](https://github.com/open-mmlab/mmsegmentation/actions)
[![codecov](https://codecov.io/gh/open-mmlab/mmsegmentation/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmsegmentation)
[![license](https://img.shields.io/github/license/open-mmlab/mmsegmentation.svg)](https://github.com/open-mmlab/mmsegmentation/blob/master/LICENSE)
[![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmsegmentation.svg)](https://github.com/open-mmlab/mmsegmentation/issues)
[![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmsegmentation.svg)](https://github.com/open-mmlab/mmsegmentation/issues)

文档: https://mmsegmentation.readthedocs.io/zh_CN/latest

[English](README.md) | 简体中文

## 简介

MMSegmentation 是一个基于 PyTorch 的语义分割开源工具箱。它是 OpenMMLab 项目的一部分。

主分支代码目前支持 PyTorch 1.5 以上的版本。

![示例图片](resources/seg_demo.gif)

### 主要特性

- **统一的基准平台**

  我们将各种各样的语义分割算法集成到了一个统一的工具箱，进行基准测试。
- **模块化设计**

  MMSegmentation 将分割框架解耦成不同的模块组件，通过组合不同的模块组件，用户可以便捷地构建自定义的分割模型。
- **丰富的即插即用的算法和模型**

  MMSegmentation 支持了众多主流的和最新的检测算法，例如 PSPNet，DeepLabV3，PSANet，DeepLabV3+ 等.
- **速度快**

  训练速度比其他语义分割代码库更快或者相当。

## 开源许可证

该项目采用 [Apache 2.0 开源许可证](LICENSE)。

## 更新日志

最新版本 v0.21.1 在 2022.2.9 发布。
如果想了解更多版本更新细节和历史信息，请阅读[更新日志](docs/en/changelog.md)。

## 基准测试和模型库

测试结果和模型可以在[模型库](docs/zh_cn/model_zoo.md)中找到。

已支持的骨干网络：

- [X]  ResNet (CVPR'2016)
- [X]  ResNeXt (CVPR'2017)
- [X]  [HRNet (CVPR'2019)](configs/hrnet)
- [X]  [ResNeSt (ArXiv'2020)](configs/resnest)
- [X]  [MobileNetV2 (CVPR'2018)](configs/mobilenet_v2)
- [X]  [MobileNetV3 (ICCV'2019)](configs/mobilenet_v3)
- [X]  [Vision Transformer (ICLR'2021)](configs/vit)
- [X]  [Swin Transformer (ICCV'2021)](configs/swin)
- [X]  [Twins (NeurIPS'2021)](configs/twins)

已支持的算法：

- [X]  [FCN (CVPR'2015/TPAMI'2017)](configs/fcn)
- [X]  [ERFNet (T-ITS'2017)](configs/erfnet)
- [X]  [UNet (MICCAI'2016/Nat. Methods'2019)](configs/unet)
- [X]  [PSPNet (CVPR'2017)](configs/pspnet)
- [X]  [DeepLabV3 (ArXiv'2017)](configs/deeplabv3)
- [X]  [BiSeNetV1 (ECCV'2018)](configs/bisenetv1)
- [X]  [PSANet (ECCV'2018)](configs/psanet)
- [X]  [DeepLabV3+ (CVPR'2018)](configs/deeplabv3plus)
- [X]  [UPerNet (ECCV'2018)](configs/upernet)
- [X]  [ICNet (ECCV'2018)](configs/icnet)
- [X]  [NonLocal Net (CVPR'2018)](configs/nonlocal_net)
- [X]  [EncNet (CVPR'2018)](configs/encnet)
- [X]  [Semantic FPN (CVPR'2019)](configs/sem_fpn)
- [X]  [DANet (CVPR'2019)](configs/danet)
- [X]  [APCNet (CVPR'2019)](configs/apcnet)
- [X]  [EMANet (ICCV'2019)](configs/emanet)
- [X]  [CCNet (ICCV'2019)](configs/ccnet)
- [X]  [DMNet (ICCV'2019)](configs/dmnet)
- [X]  [ANN (ICCV'2019)](configs/ann)
- [X]  [GCNet (ICCVW'2019/TPAMI'2020)](configs/gcnet)
- [X]  [FastFCN (ArXiv'2019)](configs/fastfcn)
- [X]  [Fast-SCNN (ArXiv'2019)](configs/fastscnn)
- [X]  [ISANet (ArXiv'2019/IJCV'2021)](configs/isanet)
- [X]  [OCRNet (ECCV'2020)](configs/ocrnet)
- [X]  [DNLNet (ECCV'2020)](configs/dnlnet)
- [X]  [PointRend (CVPR'2020)](configs/point_rend)
- [X]  [CGNet (TIP'2020)](configs/cgnet)
- [X]  [BiSeNetV2 (IJCV'2021)](configs/bisenetv2)
- [X]  [STDC (CVPR'2021)](configs/stdc)
- [X]  [SETR (CVPR'2021)](configs/setr)
- [X]  [DPT (ArXiv'2021)](configs/dpt)
- [X]  [Segmenter (ICCV'2021)](configs/segmenter)
- [X]  [SegFormer (NeurIPS'2021)](configs/segformer)

已支持的数据集：

- [X]  [Cityscapes](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#cityscapes)
- [X]  [PASCAL VOC](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#pascal-voc)
- [X]  [ADE20K](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#ade20k)
- [X]  [Pascal Context](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#pascal-context)
- [X]  [COCO-Stuff 10k](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#coco-stuff-10k)
- [X]  [COCO-Stuff 164k](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#coco-stuff-164k)
- [X]  [CHASE_DB1](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#chase-db1)
- [X]  [DRIVE](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#drive)
- [X]  [HRF](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#hrf)
- [X]  [STARE](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#stare)
- [X]  [Dark Zurich](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#dark-zurich)
- [X]  [Nighttime Driving](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#nighttime-driving)
- [X]  [LoveDA](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#loveda)
- [X]  [Potsdam](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#isprs-potsdam)
- [X]  [Vaihingen](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#isprs-vaihingen)
- [X]  [iSAID](https://github.com/open-mmlab/mmsegmentation/blob/master/docs/zh_cn/dataset_prepare.md#isaid)

## 安装

请参考[快速入门文档](docs/zh_cn/get_started.md#installation)进行安装，参考[数据集准备](docs/zh_cn/dataset_prepare.md)处理数据。

## 快速入门

请参考[训练教程](docs/zh_cn/train.md)和[测试教程](docs/zh_cn/inference.md)学习 MMSegmentation 的基本使用。
我们也提供了一些进阶教程，内容覆盖了[增加自定义数据集](docs/zh_cn/tutorials/customize_datasets.md)，[设计新的数据预处理流程](docs/zh_cn/tutorials/data_pipeline.md)，[增加自定义模型](docs/zh_cn/tutorials/customize_models.md)，[增加自定义的运行时配置](docs/zh_cn/tutorials/customize_runtime.md)。
除此之外，我们也提供了很多实用的[训练技巧说明](docs/zh_cn/tutorials/training_tricks.md)和模型部署相关的[有用的工具](docs/zh_cn/useful_tools.md)。

同时，我们提供了 Colab 教程。你可以在[这里](demo/MMSegmentation_Tutorial.ipynb)浏览教程，或者直接在 Colab 上[运行](https://colab.research.google.com/github/open-mmlab/mmsegmentation/blob/master/demo/MMSegmentation_Tutorial.ipynb)。

## 引用

如果你觉得本项目对你的研究工作有所帮助，请参考如下 bibtex 引用 MMSegmentation。

```bibtex
@misc{mmseg2020,
    title={{MMSegmentation}: OpenMMLab Semantic Segmentation Toolbox and Benchmark},
    author={MMSegmentation Contributors},
    howpublished = {\url{https://github.com/open-mmlab/mmsegmentation}},
    year={2020}
}
```

## 贡献指南

我们感谢所有的贡献者为改进和提升 MMSegmentation 所作出的努力。请参考[贡献指南](.github/CONTRIBUTING.md)来了解参与项目贡献的相关指引。

## 致谢

MMSegmentation 是一个由来自不同高校和企业的研发人员共同参与贡献的开源项目。我们感谢所有为项目提供算法复现和新功能支持的贡献者，以及提供宝贵反馈的用户。 我们希望这个工具箱和基准测试可以为社区提供灵活的代码工具，供用户复现已有算法并开发自己的新模型，从而不断为开源社区提供贡献。

## OpenMMLab 的其他项目

- [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab 计算机视觉基础库
- [MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab 图像分类工具箱
- [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab 目标检测工具箱
- [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab 新一代通用 3D 目标检测平台
- [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab 语义分割工具箱
- [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab 新一代视频理解工具箱
- [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab 一体化视频目标感知平台
- [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab 姿态估计工具箱
- [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab 图像视频编辑工具箱
- [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab 全流程文字检测识别理解工具包
- [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab 生成模型工具箱
- [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab 光流估计工具箱与测试基准
- [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab 少样本学习工具箱与测试基准
- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 人体参数化模型工具箱与测试基准
- [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab 自监督学习工具箱与测试基准
- [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab 模型压缩工具箱与测试基准
- [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab 模型部署框架
- [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab 旋转框检测工具箱与测试基准

## 欢迎加入 OpenMMLab 社区

扫描下方的二维码可关注 OpenMMLab 团队的 [知乎官方账号](https://www.zhihu.com/people/openmmlab)，加入 [OpenMMLab 团队](https://jq.qq.com/?_wv=1027&k=aCvMxdr3) 以及 [MMSegmentation](https://jq.qq.com/?_wv=1027&k=ukevz6Ie) 的 QQ 群。

<div align="center">
 <img src="docs/zh_cn/imgs/zhihu_qrcode.jpg" height="400" />  <img src="docs/zh_cn/imgs/qq_group_qrcode.jpg" height="400" />  <img src="docs/zh_cn/imgs/seggroup_qrcode.jpg" height="400" />
 </div>

我们会在 OpenMMLab 社区为大家

- 📢 分享 AI 框架的前沿核心技术
- 💻 解读 PyTorch 常用模块源码
- 📰 发布 OpenMMLab 的相关新闻
- 🚀 介绍 OpenMMLab 开发的前沿算法
- 🏃 获取更高效的问题答疑和意见反馈
- 🔥 提供与各行各业开发者充分交流的平台

干货满满 📘，等你来撩 💗，OpenMMLab 社区期待您的加入 👬
