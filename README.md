# deeplabv3+ implemented in Pytorch 4.0
This repository is forked from https://github.com/jfzhang95/pytorch-deeplab-xception, and I add the vocaug dataset, and use new trainning strategy.

### TODO
- [x] Basic deeplab v3+ model, using modified xception as backbone
- [x] Training deeplab v3+ on Pascal VOC 2012, SBD, Cityscapes datasets
- [x] Results evaluation on Pascal VOC 2012 test set
- [x] Deeplab v3+ model using resnet as backbone
- [x] Trainning deeplab v3+ on VOCAug dataset


### Introduction
This is a PyTorch(0.4.0) implementation of [DeepLab-V3-Plus](https://arxiv.org/pdf/1802.02611). It
can use Modified Aligned Xception and ResNet as backbone. Currently, we can train DeepLab V3 Plus
using Pascal VOC 2012, Pascal VOCAug, SBD and Cityscapes datasets.

![Results](doc/results.png)


### Installation
The code was tested with Anaconda and Python 3.5. After installing the Anaconda environment:

0. Clone the repo:
    ```Shell
    git clone git@github.com:dontLoveBugs/deeplabv3plus_pytorch.git
    cd deeplabv3plus_pytorch
    ```

1. Install dependencies:

    For PyTorch dependency, see [pytorch.org](https://pytorch.org/) for more details.

    For custom dependencies:
    ```Shell
    pip install matplotlib pillow tensorboardX
    ```

2. Configure your dataset path in [mypath.py](https://github.com/jfzhang95/pytorch-deeplab-xception/blob/master/mypath.py).

3. You can train deeplab v3+ using xception or resnet as backbone.

    To train DeepLabV3+ on Pascal VOC 2012, please do:
    ```Shell
    python train.py
    ```

    To train it on Cityscapes, please do:
    ```Shell
    python train_cityscapes.py
    ```



