# Motion Aware Event Representation-driven Image Deblurring-ECCV 2024
This is the official code of Motion Aware Event Representation-driven Image Deblurring.
Code coming soon...

## Motion Aware Event Representation-driven Image Deblurring
> Traditional image deblurring struggles with high-quality reconstruction due to limited motion data from single blurred images. Excitingly, the high-temporal resolution of event cameras records motion
more precisely in a different modality, transforming image deblurring.
However, many event camera-based methods, which only care about the
final value of the polarity accumulation, ignore the influence of the absolute intensity change where events generate so fall short in perceiving
motion patterns and effectively aiding image reconstruction. To overcome
this, in this work, we propose a new event preprocessing technique that
accumulates the deviation from the initial moment each time the event is
updated. This process can distinguish the order of events to improve the
perception of object motion patterns. To complement our proposed event
representation, we create a recurrent module designed to meticulously
extract motion features across local and global time scales. To further
facilitate the event feature and image feature integration, which assists in
image reconstruction, we develop a bi-directional feature alignment and
fusion module. This module works to lessen inter-modal inconsistencies.
Our approach has been thoroughly tested through rigorous experiments
carried out on several datasets with different distributions. These trials have delivered promising results, with our method achieving top-tier
performance in both quantitative and qualitative assessments.

## Overview

This is the overview of our network's architecture:
![image](https://github.com/ZhijingS/DA_event_deblur/blob/main/network.png)
The differences of our Deviation Accumulation(DA) event representation and other Polarity Accumulation(PA) representation:
![image](https://github.com/ZhijingS/DA_event_deblur/blob/main/DArep.png)
![image](https://github.com/ZhijingS/DA_event_deblur/blob/main/algo.png)
See more details in our paper.

## Installation

-TODO

## Dataset & Data Preprocess

-TODO

## Evaluation
The quantitative results of our method on GoPro, HS-ERGB and REBlur test datasets.
#### Pretrained Model Download 

- TODO

#### Test

- TODO

## Training

- TODO

## Citation

If you find our work useful in your research, please consider citing:

```
@InProceedings{Xu_2024_CVPR,
    author    = {Xu, Senyan and Sun, Zhijing and Zhu, Jiaying and Zhu, Yurui and Fu, Xueyang and Zha, Zheng-Jun},
    title     = {DemosaicFormer: Coarse-to-Fine Demosaicing Network for HybridEVS Camera},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
    month     = {June},
    year      = {2024},
    pages     = {1126-1135}
}
```

## Contact

Should you have any question, please contact [syxu@mail.ustc.edu.cn](syxu@mail.ustc.edu.cn)

**Acknowledgment:** This code is based on the [BasicSR](https://github.com/xinntao/BasicSR) toolbox.
