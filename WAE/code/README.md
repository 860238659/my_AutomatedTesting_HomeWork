# Code for Wireframe-based UI Design Search Through Image Autoencoder


#### Image Preprocessing 图像预处理

use *wirification.py*

This code is implemented using PyThon2

Please read and modify it as you need by yourself.

此代码是使用 PyThon2 实现的

请阅读并根据需要自行修改。


#### Model Training and Testing 模型训练和测试

To use this code in your dataset, you may need to modify the *dataloader.py* to read your wireframe/source uis. 
You could first use the toy sample to be familiar with the input/output.

要在数据集中使用此代码，您可能需要修改dataloader.py来读取您的线框源代码ui。

您可以先使用玩具样品来熟悉输入/输出。

### Requirement
```
python3 -m pip install -r requirements.txt
```

### Training

```
python3 train.py \
--data_root "train_data" \
--cache_root "results/run/cache" \
--model_dir "results/run" \
--epochs 10

```


### Testing

```
python3 test.py \
--data_root "." \
--cache_root "results/run/cache" \
--model_dir "results/run" \
--checkpoint "results/run/state_dict_final.pth" \
--use_flann 0 \
--test_dir "test_data" \
--result_dir "results/test_result" \
```

*See more options in opts.py*

