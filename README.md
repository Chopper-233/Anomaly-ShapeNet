# Anomaly-ShapeNet: A Synthetic Dataset of Point Cloud Anomaly Detection

Wenqiao Li, Xiaohao Xu, Yao Gu

Our paper is under review. [[Paper]](https://arxiv.org/abs/2311.14897)

# Overview
This project provides a synthetic dataset for point cloud anomaly detection. We only provide 3D point clouds for training and testing 3D anomaly detection algorithms.
Note that we expanded from the original 40 classes to 50 classes and put the new 10 classes in the ‘new’ folders.
Considering our paper is under review at the early stage, the algorithm(IMRNet) will be released after our dataset.If you have any problem for the code, you can directly email me. 


# Anomaly-ShapeNet

<img src="./examples.png" width=900 alt="Dataset" align=center>


## Summary
+ overview of Anomaly-ShapeNet

Anomaly-ShapeNet comprises a total of 1600 samples which are distributed across 40(+10) distinct categories. There are six kinds of anomalies, including bulge, concavity, crack, holes, and broken. All the obj or pcd file have been watertighted before to obtain a more smooth surface.


## Download

+ To download our Anomaly-ShapeNet dataset (Dataset for training and evaluation, pcd&obj format), click [Anomaly-ShapeNet.zip(baidu disk: case)](https://pan.baidu.com/s/1Nm50WIU_jx5viozwe59HsQ?pwd=case)or[Anomaly-ShapeNet.zip(Google drive)(https://drive.google.com/file/d/16R8b39Os97XJOenB4bytxlV4vd_5dn0-/view?usp=sharing)



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
### IMRNet

code is coming soon...

### Checkpoint

coming soon...
                                                                                                    |
## Thanks

Our dataset and code is built on [Real3D-AD](https://github.com/eliahuhorwitz/3D-ADS) and [M3DM](https://github.com/nomewang/M3DM), thanks for their excellent works!

## License
The dataset is released under the CC BY 4.0 license.
