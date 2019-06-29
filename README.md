# Efficient Mask R-CNN for Object Detection and Segmentation


### TODO:
- [x] Integrate basic efficient net b0.
- [x] Add drop-connect, squeeze and excitation layers.
- [x] Training and re-loading pretrained weights for the entire network.
- [ ] Add generator for efficient nets from b1 - b7
- [ ] Allow loading pre-trained weights for efficient net.

## Setup
- Model: mask_rcnn
- Feature Extractor: efficient_net
- Dataset: COCO 2017
- Task: Instance Segmentation

## Requirements
- See requirements.txt

## Getting Started

```
# Setup all dependencies
python3 setup.py install

# Setup training parameters
# configure in samples/coco/coco.py, additionally refer to mrcnn/config.py

# Download the dataset and start training
python3 samples/coco/coco.py train --download=True

# Resume training from previous run
python3 samples/coco/coco.py train --model=last

# Evaluate trained model
python3 samples/coco/coco.py evaluate --model=last

# More options coming soon
```


## References:

Papers:
- https://arxiv.org/pdf/1905.11946v2.pdf
- https://arxiv.org/abs/1703.06870

Blogs:

- https://engineering.matterport.com/splash-of-color-instance-segmentation-with-mask-r-cnn-and-tensorflow-7c761e238b46

Repos:
- https://github.com/matterport/Mask_RCNN
- https://github.com/tensorflow/tpu/tree/master/models/official/efficientnet
- https://github.com/gustavz/Mobile_Mask_RCNN

Errors:
- https://github.com/matterport/Mask_RCNN/issues/958
- https://github.com/tensorflow/tensorflow/issues/29073
- https://github.com/ayufan-rock64/linux-build/issues/136