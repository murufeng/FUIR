<details> <summary> Image Derain - Rain13k dataset </summary>

* prepare data

  * ```mkdir ./datasets/Rain13k```

  * download the [train](https://drive.google.com/drive/folders/1Hnnlc5kI0v9_BtfMytC2LR5VpLAFZtVe?usp=sharing) set and [test](https://drive.google.com/drive/folders/1PDWggNh8ylevFmrjo-JEvlmqsDlWWvZs?usp=sharing) 

  * it should be like

    ```
    ./datasets/
    ./datasets/Rain13k/
    ./datasets/Rain13k/train/
    ./datasets/Rain13k/train/input/
    ./datasets/Rain13k/train/target/
    ./datasets/Rain13k/test/
    ./datasets/Rain13k/test/Test100/
    ./datasets/Rain13k/test/Rain100H/
    ./datasets/Rain13k/test/Rain100L/
    ./datasets/Rain13k/test/Test2800/
    ./datasets/Rain13k/test/Test1200/
    ```

* eval

    * Save your pretrain model weight to ./experiments/pretrained_models/pretrain_model.pth
    
    * For Test100:

      * ```python basicsr/test.py -opt options/test/Rain13k/model-Test100.yml``` 
      
    * For Rain100H

      * ```python basicsr/test.py -opt options/test/Rain13k/model-Rain100H.yml``` 
    * For Rain100L

      * ```python basicsr/test.py -opt options/test/Rain13k/model-Rain100L.yml``` 
    * For Test2800

      * ```python basicsr/test.py -opt options/test/Rain13k/model-Test2800.yml``` 
    * For Test1200

      * ```python basicsr/test.py -opt options/test/Rain13k/model-Test1200.yml``` 

* train

    * ```python -m torch.distributed.launch --nproc_per_node=8 --master_port=4321 basicsr/train_rain.py -opt options/train/Rain13k/model.yml --launcher pytorch```

</details>