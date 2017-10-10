# malis-pytorch: Malis layer implemented in pytorch
## MalisLoss Intallation
1. Install library dependencies:
```
    conda install cython boost
```
2. modify `setup.py`
```
    CONDA_ENV_INCLUDE=YOUR_PATH
```
3. compile
```
    ./make.sh
```
## Pytorch Package for Unet3D 
1. Basic module 
    - T_data.py: dataLoader for volume data
    - T_model.py: unet3D (with and without BatchNorm)
    - T_pruner.py: channel pruning (in progress)
2. Example
    - E_benchmark.py: benchmark speed
    - E_test.py: test on a volume
    - E_train.py: train on a volume
    - E_prune.py: channel prune model

## Reference:
1. [malis: cython implementation](https://github.com/TuragaLab/malis)
2. [malis: caffe layer implementation](https://github.com/naibaf7/caffe/blob/master/src/caffe/layers/malis_loss_layer.cpp)
3. [unet: pytorch
   implementation](https://github.com/meetshah1995/pytorch-semseg/blob/master/ptsemseg/models/unet.py)