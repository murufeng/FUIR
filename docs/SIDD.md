# reproduce the SIDD dataset results 

### 1. Data Preparation
* prepare data

  * ```mkdir ./datasets/SIDD ```
  
##### Download the train set and place it in ```./datasets/SIDD/Data```:

* [google drive](https://drive.google.com/file/d/1UHjWZzLPGweA9ZczmV8lFSRcIxqiOVJw/view?usp=sharing) or [百度网盘](https://pan.baidu.com/s/1EnBVjrfFBiXIRPBgjFrifg?pwd=sl6h), 
* ```python scripts/data_preparation/sidd.py``` to crop the train image pairs to 512x512 patches and make the data into lmdb format.

  * it should be like:
    ```bash
    ./datasets/SIDD/Data
    ./datasets/SIDD/train
    ./datasets/SIDD/val
    ./datasets/SIDD/test
    ./datasets/SIDD/test/ValidationNoisyBlocksSrgb.mat
    ./datasets/SIDD/test/ValidationGtBlocksSrgb.mat
    ```
  
 * ```python scripts/data_preparation/sidd.py``` 
 * to crop the train image pairs to 512x512 patches and make the data into lmdb format.


##### Download the evaluation data (in lmdb format) and place it in ```./datasets/SIDD/val/```:

  * [google drive](https://drive.google.com/file/d/1gZx_K2vmiHalRNOb1aj93KuUQ2guOlLp/view?usp=sharing) or [百度网盘](https://pan.baidu.com/s/1I9N5fDa4SNP0nuHEy6k-rw?pwd=59d7), 
  * it should be like ```./datasets/SIDD/val/input_crops.lmdb``` and ```./datasets/SIDD/val/gt_crops.lmdb```



### 2. Training

* Your model:

  ```
  python -m torch.distributed.launch --nproc_per_node=8 --master_port=4321 basicsr/train.py -opt options/train/SIDD/xxxx.yml --launcher pytorch
  ```

* 8 gpus by default. Set ```--nproc_per_node``` to # of gpus for distributed validation.

 

### 3. Evaluation


##### Save your pretrain model weight in ```./experiments/pretrained_models/```

##### Testing on SIDD dataset	

  * Your model:

```
python -m torch.distributed.launch --nproc_per_node=1 --master_port=4321 basicsr/test.py -opt ./options/test/SIDD/xxx.yml --launcher pytorch
```

* Test by a single gpu by default. Set ```--nproc_per_node``` to # of gpus for distributed validation.



