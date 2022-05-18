# reproduce the GoPro dataset results 

### 1. Data Preparation

##### Download the train set and place it in ```./datasets/GoPro/train```:

* [google drive](https://drive.google.com/file/d/1zgALzrLCC_tcXKu_iHQTHukKUVT1aodI/view?usp=sharing) or [百度网盘](https://pan.baidu.com/s/1fdsn-M5JhxCL7oThEgt1Sw?pwd=9d26)
* it should be like ```./datasets/GoPro/train/input ``` and ```./datasets/GoPro/train/target```
* ```python scripts/data_preparation/gopro.py``` to crop the train image pairs to 512x512 patches and make the data into lmdb format.

##### Download the evaluation data (in lmdb format) and place it in ```./datasets/GoPro/test/```:

  * [google drive](https://drive.google.com/file/d/1abXSfeRGrzj2mQ2n2vIBHtObU6vXvr7C/view?usp=sharing) or [百度网盘](https://pan.baidu.com/s/1oZtEtYB7-2p3fCIspky_mw?pwd=rmv9)
  * it should be like ```./datasets/GoPro/test/input.lmdb``` and ```./datasets/GoPro/test/target.lmdb```



### 2. Training

* Model 

  ```
  python -m torch.distributed.launch --nproc_per_node=8 --master_port=4321 basicsr/train.py -opt options/train/GoPro/your_model.yml --launcher pytorch
  ```

* 8 gpus by default. Set ```--nproc_per_node``` to # of gpus for distributed validation.

  
### 3. Evaluation

##### Save your pretrain model weight in ```./experiments/pretrained_models/```

##### Testing on GoPro dataset	

* Model

  ```
  python -m torch.distributed.launch --nproc_per_node=1 --master_port=4321 basicsr/test.py -opt ./options/test/GoPro/your_model.yml --launcher pytorch
  ```

* Test by a single gpu by default. Set ```--nproc_per_node``` to # of gpus for distributed validation.

