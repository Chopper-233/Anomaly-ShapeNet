# Anomaly-ShapeNet: A Synthetic Dataset of Point Cloud Anomaly Detection

Wenqiao Li, Xiaohao Xu, Yao Gu, Bozhong Zheng, Shenghua Gao, Yingna Wu
## 🧩News
\textbf{1.Check out our Anomaly-ShapeNet follow-up dataset Mulsen-AD here!}(CVPR2025)[[Link]](https://github.com/ZZZBBBZZZ/MulSen-AD/))
\textbf{2.Check out our IMRNet follow-up algorithm here PASDF here!(ICCV2025)}[[Link]](https://github.com/ZZZBBBZZZ/PASDF))
## Introduction
This project provides a synthetic dataset for point cloud anomaly detection. We provide 3D point clouds and meshs for training and testing 3D anomaly detection algorithms.
Note that we expanded from the original 40 classes to 50 classes and put the new 10 classes in the ‘new’ folders.Our paper can be found here.[[Paper]](https://arxiv.org/abs/2311.14897)


## Data description

<img src="./examples.png" width=900 alt="Dataset" align=center>

+ overview of Anomaly-ShapeNet

Anomaly-ShapeNet comprises a total of 1600 samples which are distributed across 40(+10) distinct categories. There are six kinds of anomalies, including bulge, concavity, crack, holes, and broken. All the obj or pcd file have been watertighted before to obtain a more smooth surface.
| Datasets |   Category numbers  | Anomaly types| Train num(1cls) |  Test num(1cls) | Point num | Anomaly portion | 
|--------------|:----:|:-----:|:-------:|:-------:|:------:|:-------:|
| Anomaly-ShapeNet |    50    |     6    |    4    |   15~24   |   8K~30K   |   1%~7%   |


## Download

+ To download our Anomaly-ShapeNet dataset (Dataset for training and evaluation, pcd&obj format), click [Anomaly-ShapeNet.zip(baidu disk: case)](https://pan.baidu.com/s/1Nm50WIU_jx5viozwe59HsQ?pwd=case) or (hugging face)(https://huggingface.co/datasets/Chopper233/Anomaly-ShapeNet)



### Data preparation
- Download Anomaly-ShapeNet-v2.zip and extract into `./dataset/pcd`
```
pcd
├── ashtray0
    ├── train
        ├── *template.pcd
        ...
    ├── test
        ├── 1_bulge.pcd
        ├── 2_concavity.pcd
        ...
    ├── GT
        ├── 1_bulge.txt
        ├── 2_sink.txt
        ... 
├── bag0
...
```
## Benchmark
Our benchmark for Anomaly ShapaNet and Real3D-AD are listed here [Benchmark](https://github.com/Chopper-233/Anomaly-ShapeNet/blob/main/Benchmark.pdf). Some metrics like P-AP for Anomaly-ShapeNet is ignored because they are not suitable for our dataset.
## Citation
Please cite the following paper if this dataset helps your project:

```bibtex
@InProceedings{Li_2024_CVPR,
    author    = {Li, Wenqiao and Xu, Xiaohao and Gu, Yao and Zheng, Bozhong and Gao, Shenghua and Wu, Yingna},
    title     = {Towards Scalable 3D Anomaly Detection and Localization: A Benchmark via 3D Anomaly Synthesis and A Self-Supervised Learning Network},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    month     = {June},
    year      = {2024},
    pages     = {22207-22216}
}
```
## Thanks

Our dataset and code are built on [ShapeNet](https://shapenet.org/) and [PointMAE](https://github.com/Pang-Yatian/Point-MAE), thanks for their excellent works!

## License
The dataset is released under the CC BY 4.0 license.
