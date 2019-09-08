# Learning Adaptive Hierarchical Cuboid Abstractions of 3D Shape Collections

This is the TensorFlow implementation of ["Learning Adaptive Hierarchical Cuboid Abstractions of 3D Shape Collections"](https://isunchy.github.io/projects/cuboid_abstraction.html) by Chun-Yu Sun, Qian-Fang Zou, Xin Tong, Yang Liu, SIGGRAPH Asia 2019. The code is released under the MIT license.

<img src="teaser.png" alt="teaser" width=800px; height=373px;/>

## Setup

Pre-prequisites

        Python == 3.6
        TensorFlow == 1.12

## Experiments


### Data Preparation

### Initial Training

To start the initial training, run

        $ python initial_training.py --log_dir /path/to/save/weights --cache_folder /path/to/save/tmp_results 

During training, the network outputs intermediate data into these folders:

- ``log_dir``: Training logs which can be visualized using Tensorboard and network snapshots which can be used in evaluation.
- ``cache_folder``: Cuboids visualization during training.

To test a trained model, run

        $ python initial_training.py --ckpt /path/to/snapshots --cache_folder /path/to/save/test_results --test

### Iterative Training



## Citation

If you use our code for research, please cite our paper:
```
@article{sun2019abstraction,
title     = {Learning Adaptive Hierarchical Cuboid Abstractions of 3D Shape Collections},
author    = {Sun, Chunyu and Zou, Qianfang and Tong, Xin and Liu, Yang},
journal   = {ACM Transactions on Graphics (SIGGRAPH Asia)},
volume    = {38},
number    = {6},
year      = {2019},
publisher = {ACM}
}
```

## Contact

Please contact us (Chunyu Sun sunchyqd@gmail.com, Yang Liu yangliu@microsoft.com) if you have any problem about our implementation or request to all the datasets.
