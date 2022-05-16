# Installation

This repository is built in PyTorch 1.8.0 and tested on Ubuntu 18.04 environment (Python3.7, CUDA11.2, cuDNN7.6).
Follow these intructions

1. Clone our repository
```
git clone https://github.com/murufeng/FUIR.git
cd FUIR
```

2. Make conda environment
```
conda create -n pytorch1.8.0_FUIR python=3.7
conda activate pytorch1.8.0_FUIR
```

3. Install dependencies
```
conda install pytorch=1.8.0 torchvision cudatoolkit=11.2 -c pytorch
pip install matplotlib scikit-learn scikit-image opencv-python yacs joblib natsort h5py tqdm
pip install einops gdown addict future lmdb numpy pyyaml requests scipy tb-nightly yapf lpips
```
