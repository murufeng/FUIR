# reproduce the REDS dataset results 

### 1. Data Preparation

##### Download the train set and place it in ```./datasets/REDS/train```:

* google drive ([link](https://drive.google.com/file/d/1VTXyhwrTgcaUWklG-6Dh4MyCmYvX39mW/view) and [link](https://drive.google.com/file/d/1YLksKtMhd2mWyVSkvhDaDLWSc1qYNCz-/view)) or SNU CVLab Server ([link](http://data.cv.snu.ac.kr:8008/webdav/dataset/REDS/train_blur_jpeg.zip) and [link](http://data.cv.snu.ac.kr:8008/webdav/dataset/REDS/train_sharp.zip))
* it should be like ```./datasets/REDS/train/train_blur_jpeg ``` and ```./datasets/REDS/train/train_sharp```
* ```python scripts/data_preparation/reds.py``` to make the data into lmdb format.

##### Download the evaluation data (in lmdb format) and place it in ```./datasets/REDS/val/```:

  * [google drive](https://drive.google.com/file/d/1_WPxX6mDSzdyigvie_OlpI-Dknz7RHKh/view?usp=sharing) or [百度网盘](https://pan.baidu.com/s/1yUGdGFHQGCB5LZKt9dVecw?pwd=ikki),
  * it should be like ```./datasets/REDS/val/blur_300.lmdb``` and ```./datasets/REDS/val/sharp_300.lmdb```



### 2. Training

* Model:

  ```
  python -m torch.distributed.launch --nproc_per_node=8 --master_port=4321 basicsr/train.py -opt options/train/REDS/xxxx.yml --launcher pytorch
  ```

* 8 gpus by default. Set ```--nproc_per_node``` to # of gpus for distributed validation.

  


### 3. Evaluation

##### Save your pretrain model weight in ```./experiments/pretrained_models/``` 

##### Testing on REDS dataset	

  * Model:
```
python -m torch.distributed.launch --nproc_per_node=1 --master_port=4321 basicsr/test.py -opt ./options/test/REDS/xxxx.yml --launcher pytorch
```

* Test by a single gpu by default. Set ```--nproc_per_node``` to # of gpus for distributed validation.

