# IROS2019 lifelong Robotic Vision---lifelong object recognition challenge Baseline Model
This is a PyTorch implementation of baseline model of IROS2019 lifelong object recognition challenge ([link](https://lifelong-robotic-vision.github.io/competition/Object-Recognition.html)).
This repository provides:
* Pretrained models for specific batches (batch 5 and batch 6's model for multitask training scheme, batch 9's model for finetuning scheme)
* MobileNetV2 [[1](##References)]  backbone for the task (using random crop for input images)
* Script for running the baseline model (with dataloader module for reference)

## Requirements
-The current version of the code has been tested with following libs:

* `python 3.7`
* `numpy 1.16.2`
* `pandas 0.24.2`
* `pytorch 1.1.0`
* `torchvision 0.2.2`
* `PIL 6.0.0`

- recommend install in virtual environment
```
$ conda create -n yourenvname python=3.7 anaconda
```
- Install the required the packages inside the virtual environment
```
$ source activate yourenvname
$ pip install -r requirements.txt
```


## Running the baseline model

Script for running the baseline model can be run with `evaluate.py`. Here `testset_path` and `output_path`is the path you stored your testset data and output prediction results for each batch. Results files will generated under specified output path. 
```
python3 evaluate.py testset_path output_path
```

## References

[1] Sandler, Mark, et al. "Mobilenetv2: Inverted residuals and linear bottlenecks." Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2018. [[pdf](http://openaccess.thecvf.com/content_cvpr_2018/papers/Sandler_MobileNetV2_Inverted_Residuals_CVPR_2018_paper.pdf)]


