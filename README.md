# Project
![Architecture](https://i.imgur.com/2imjdUf.png)

Diffusion-based vector image generator. Aims for a practical application.
[Click here to see more.](https://www.notion.so/parkcymil/14c2655becda80e8a041d63471a814ee)

## Prerequisite
- Python 3.9
- [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit)
- [NVIDIA cuDNN](https://developer.nvidia.com/cudnn)

## Install modules
If you don't use anaconda, use pip to install the modules. (Not recommended)

Make sure the CUDA Toolkit 12.4 is installed before you proceed!

```shell
conda install pytorch torchvision torchaudio pytorch-cuda=12.4 -c pytorch -c nvidia
conda install -c conda-forge accelerate
conda install -c conda-forge diffusers
conda install conda-forge::transformers
pip install xformers --index-url https://download.pytorch.org/whl/cu124
pip install compel sentencepiece protobuf nltk
```

## Update submodules
```shell
git submodule update --init --recursive
```

Refer [this document](https://github.com/BachiLi/diffvg?tab=readme-ov-file#install) to install and build DiffVG.


## Troubleshoot
- [If system fails to load libcudnn_cnn_infer.so.8 (WSL only)](https://github.com/microsoft/WSL/issues/8587)
