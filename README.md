# pytorch-gpu-speed

This repository reports the speed of Pytorch according to the pytorch version, gpu types, cuda version, etc. The code refers to [this issue](https://github.com/pytorch/pytorch/issues/47039). More data is weclome!!!

|package name| gpu type| pytorch version |  conv1d or conv2d | benchmark | result(ms/iter) |
|-----------|-----------|-----------|-----------|-----------|-----------|
|py3.8_cuda11.3_cudnn8.3.2_0| GTX 1080| 1.12.1| conv1d| False | 0.270|
||||conv1d|True|0.269|
||||conv2d|False|2.883|
||||conv2d|True|2.844|
||GTX 1080 Ti||conv1d|False|0.283|
||||conv1d|True|0.281|
||||conv2d|False|2.225|
||||conv2d|True|2.079|
||TITAN Xp||conv1d|False|0.282|
||||conv1d|True|0.277|
||||conv2d|False|2.069|
||||conv2d|True|1.951|
||Tesla V100 16G||conv1d|False|0.425|
||||conv1d|True|0.421|
||||conv2d|False|1.465|
||||conv2d|True|1.433|
||NVIDIA A100-PCIE-40GB||conv1d|False|0.463|
||||conv1d|True|0.464|
||||conv2d|False|1.547|
||||conv2d|True|0.990|
|py3.6_cuda9.2.148_cudnn7.6.3_0| GTX 1080| 1.5.0|  conv1d| False | 0.313|
||||conv1d|True|0.318|
||||conv2d|False|3.104|
||||conv2d|True|3.089|
||GTX 1080 Ti||conv1d|False|0.262|
||||conv1d|True|0.262|
||||conv2d|False|2.222|
||||conv2d|True|2.188|
||TITAN Xp||conv1d|False|0.268|
||||conv1d|True|0.267|
||||conv2d|False|2.256|
||||conv2d|True|2.083|
||Tesla V100 16G||conv1d|False|0.484|
||||conv1d|True|0.491|
||||conv2d|False|1.759|
||||conv2d|True|1.716|
|py3.6_cuda11.0.221_cudnn8.0.5_0| Tesla V100 16G| 1.7.1| conv1d| False | 0.675|
||||conv1d|True|0.616|
||||conv2d|False|6.487|
||||conv2d|True|6.483|
||A100 40G||conv1d|False|0.825|
||||conv1d|True|0.457|
||||conv2d|False|1.801|
||||conv2d|True|1.457|