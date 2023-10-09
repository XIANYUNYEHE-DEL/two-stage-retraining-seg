# two-stage-retraining-seg
## Introduction
- two-stage-retraining-seg is a segmentation method for weak label Medical segmentation, based on [EfficientSegmentation](https://github.com/Shanghai-Aitrox-Technology/EfficientSegmentation) and [nnU-Net](https://github.com/MIC-DKFZ/nnUNet)

## Installation

#### Enviroment
- Ubuntu 20.04.1 LTS
- Python 3.6(If nnU-Net requires a higher version, we recommend creating two separate environments)
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

## Weak label information

Flare2023 Datasets 2200 cases label information are summarized in `label_num.npy`. You can use this file to select 222 strong label cases(Key:'14') in 2200 weak label cases.
