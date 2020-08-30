# Mask R-CNN for Object Detection and Segmentation

This is an implementation of [Mask R-CNN](https://arxiv.org/abs/1703.06870) on Python 3, Keras, and TensorFlow. The model generates bounding boxes and segmentation masks for each instance of an object in the image. It's based on Feature Pyramid Network (FPN) and a ResNet101 backbone.

## Setup for local venv
```
$ pip install -r requirements.txt
```
If resolver has problems :
```
$ pip install -r requirements.txt --use-feature=2020-resolver
```
  
Put the last weights in the logs directory : painting20200830T0323.  
Then you are ready to go.
  
You will find the weights here :
https://drive.google.com/file/d/1UEP8uPDlCuFGiWvvyziuEH7akmNfGgZX/view?usp=sharing


## to train
```
$ cd data
$ python painting.py train --dataset=dataset --weights=last
```

## Troubleshooting
- If memory is exceeding reduce the number of images al line 66 in painting.py
- The model is compatible with tf 1.14 not 2
