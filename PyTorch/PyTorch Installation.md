# PyTorch Installation --cpu version ubuntu 18.04

```bash
conda create -n pytorch-py python=3.6
conda activate pytorch-py
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/msys2/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/
conda config --set show_channel_urls yes
conda install pytorch torchvision torchaudio cpuonly
```



# PyTorch Geometric Installation

