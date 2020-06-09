# DETR based on Detectron2

## Instructions
1. Follow detectron2's readme to install detection2
  * ```python setup.py build develop```
  * link dataset path to DETR.detectron2/datasets/
2. Run DETR
  * ```cd DETR.detectron2```
  * ```python projects/DETR/train_net.py --num-gpus 8 --config-file projects/DETR/configs/detr.res50.coco.multiscale.150e.yaml```

## Disclaimer
* I haven't add RandomCrop.
* I haven't add support for segmentaion, but it can be easily added. 

## Advantage
* Training faster
* Avoid memory leaking in official implementation
* Use backbone in detectron2
