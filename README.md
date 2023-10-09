# two-stage-retraining-seg
## Introduction
- two-stage-retraining-seg is a segmentation method for weak label Medical segmentation, based on [EfficientSegmentation](https://github.com/Shanghai-Aitrox-Technology/EfficientSegmentation) and [nnU-Net](https://github.com/MIC-DKFZ/nnUNet)

## Installation

#### Enviroment
- Ubuntu 20.04.1 LTS
- Python 3.6
- Pytorch 1.11.0+
- CUDA 11.7

1.Git clone
```
git clone https://github.com/XIANYUNYEHE-DEL/two-stage-retraining-seg
```

2.Install Nvidia Apex
- Perform the following command:
```
git clone https://github.com/NVIDIA/apex
cd apex
pip install -v --disable-pip-version-check --no-cache-dir --global-option="--cpp_ext" --global-option="--cuda_ext" ./
```

3.Install EfficientSeg dependencies
```
cd EfficientSegNet
pip install -r requirements.txt
```
3.Install nnU-Net dependencies
```
cd nnUNet
pip install -e .
```
