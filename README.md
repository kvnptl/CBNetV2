# CBNetV2: A Novel Composite Backbone Network Architecture for Object Detection

This repo contains the supported code and configuration files to reproduce object detection results of [CBNetV2](). It is based on [mmdetection](https://github.com/open-mmlab/mmdetection) and [Swin Transformer for Object Detection](https://github.com/SwinTransformer/Swin-Transformer-Object-Detection).

Contact us with tingtingliang@pku.edu.cn, wyt@pku.edu.cn.

## Results and Models

### Mask R-CNN

| Backbone | Pretrain | Lr Schd | box mAP | mask mAP | #params | FLOPs | config | log | model |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |:---: |
| Swin-T | ImageNet-1K | 1x | 43.7 | 39.8 | 48M | 267G | [config](configs/swin/mask_rcnn_swin_tiny_patch4_window7_mstrain_480-800_adamw_1x_coco.py) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.3/mask_rcnn_swin_tiny_patch4_window7_1x.log.json)/[baidu](https://pan.baidu.com/s/1bYZk7BIeFEozjRNUesxVWg) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.3/mask_rcnn_swin_tiny_patch4_window7_1x.pth)/[baidu](https://pan.baidu.com/s/19UOW0xl0qc-pXQ59aFKU5w) |
| Swin-T | ImageNet-1K | 3x | 46.0 | 41.6 | 48M | 267G | [config](configs/swin/mask_rcnn_swin_tiny_patch4_window7_mstrain_480-800_adamw_3x_coco.py) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.2/mask_rcnn_swin_tiny_patch4_window7.log.json)/[baidu](https://pan.baidu.com/s/1Te-Ovk4yaavmE4jcIOPAaw) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.2/mask_rcnn_swin_tiny_patch4_window7.pth)/[baidu](https://pan.baidu.com/s/1YpauXYAFOohyMi3Vkb6DBg) |
| Swin-S | ImageNet-1K | 3x | 48.5 | 43.3 | 69M | 359G | [config](configs/swin/mask_rcnn_swin_small_patch4_window7_mstrain_480-800_adamw_3x_coco.py) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.2/mask_rcnn_swin_small_patch4_window7.log.json)/[baidu](https://pan.baidu.com/s/1ymCK7378QS91yWlxHMf1yw) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.2/mask_rcnn_swin_small_patch4_window7.pth)/[baidu](https://pan.baidu.com/s/1V4w4aaV7HSjXNFTOSA6v6w) |

### Cascade Mask R-CNN

| Backbone | Pretrain | Lr Schd | box mAP | mask mAP | #params | FLOPs | config | log | model |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |:---: |
| Swin-T | ImageNet-1K | 1x | 48.1 | 41.7 | 86M | 745G | [config](configs/swin/cascade_mask_rcnn_swin_tiny_patch4_window7_mstrain_480-800_giou_4conv1f_adamw_1x_coco.py) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.3/cascade_mask_rcnn_swin_tiny_patch4_window7_1x.log.json)/[baidu](https://pan.baidu.com/s/1x4vnorYZfISr-d_VUSVQCA) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.3/cascade_mask_rcnn_swin_tiny_patch4_window7_1x.pth)/[baidu](https://pan.baidu.com/s/1vFwbN1iamrtwnQSxMIW4BA) |
| Swin-T | ImageNet-1K | 3x | 50.4 | 43.7 | 86M | 745G | [config](configs/swin/cascade_mask_rcnn_swin_tiny_patch4_window7_mstrain_480-800_giou_4conv1f_adamw_3x_coco.py) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.2/cascade_mask_rcnn_swin_tiny_patch4_window7.log.json)/[baidu](https://pan.baidu.com/s/1GW_ic617Ak_NpRayOqPSOA) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.2/cascade_mask_rcnn_swin_tiny_patch4_window7.pth)/[baidu](https://pan.baidu.com/s/1i-izBrODgQmMwTv6F6-x3A) |
| Swin-S | ImageNet-1K | 3x | 51.9 | 45.0 | 107M | 838G | [config](configs/swin/cascade_mask_rcnn_swin_small_patch4_window7_mstrain_480-800_giou_4conv1f_adamw_3x_coco.py) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.2/cascade_mask_rcnn_swin_small_patch4_window7.log.json)/[baidu](https://pan.baidu.com/s/17Vyufk85vyocxrBT1AbavQ) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.2/cascade_mask_rcnn_swin_small_patch4_window7.pth)/[baidu](https://pan.baidu.com/s/1Sv9-gP1Qpl6SGOF6DBhUbw) |
| Swin-B | ImageNet-1K | 3x | 51.9 | 45.0 | 145M | 982G | [config](configs/swin/cascade_mask_rcnn_swin_base_patch4_window7_mstrain_480-800_giou_4conv1f_adamw_3x_coco.py) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.2/cascade_mask_rcnn_swin_base_patch4_window7.log.json)/[baidu](https://pan.baidu.com/s/1UZAR39g-0kE_aGrINwfVHg) | [github](https://github.com/SwinTransformer/storage/releases/download/v1.0.2/cascade_mask_rcnn_swin_base_patch4_window7.pth)/[baidu](https://pan.baidu.com/s/1tHoC9PMVnldQUAfcF6FT3A) |

### RepPoints V2

| Backbone | Pretrain | Lr Schd | box mAP | mask mAP | #params | FLOPs |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Swin-T | ImageNet-1K | 3x | 50.0 | - | 45M | 283G |

### Mask RepPoints V2

| Backbone | Pretrain | Lr Schd | box mAP | mask mAP | #params | FLOPs |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Swin-T | ImageNet-1K | 3x | 50.3 | 43.6 | 47M | 292G |

**Notes**: 

- **Pre-trained models of Swin Transformer can be downloaded from [Swin Transformer for ImageNet Classification](https://github.com/microsoft/Swin-Transformer)**.
- Access code for `baidu` is `swin`.

## Usage

### Installation

Please refer to [get_started.md](https://github.com/open-mmlab/mmdetection/blob/master/docs/get_started.md) for installation and dataset preparation.

### Inference
```
# single-gpu testing
python tools/test.py <CONFIG_FILE> <DET_CHECKPOINT_FILE> --eval bbox
# or (w/ bbox_mask)
python tools/test.py <CONFIG_FILE> <DET_CHECKPOINT_FILE> --eval bbox segm

# multi-gpu testing
tools/dist_test.sh <CONFIG_FILE> <DET_CHECKPOINT_FILE> <GPU_NUM> --eval bbox
# or (w/ bbox_mask)
tools/dist_test.sh <CONFIG_FILE> <DET_CHECKPOINT_FILE> <GPU_NUM> --eval bboxsegm
```

### Training

To train a detector with pre-trained models, run:
```
# single-gpu training
python tools/train.py <CONFIG_FILE> --cfg-options model.pretrained=<PRETRAIN_MODEL> [model.backbone.use_checkpoint=True] [other optional arguments]

# multi-gpu training
tools/dist_train.sh <CONFIG_FILE> <GPU_NUM> --cfg-options model.pretrained=<PRETRAIN_MODEL> [model.backbone.use_checkpoint=True] [other optional arguments] 
```
For example, to train a Cascade Mask R-CNN model with a `Swin-T` backbone and 8 gpus, run:
```
tools/dist_train.sh configs/swin/cascade_mask_rcnn_swin_tiny_patch4_window7_mstrain_480-800_giou_4conv1f_adamw_3x_coco.py 8 --cfg-options model.pretrained=<PRETRAIN_MODEL> 
```

**Note:** `use_checkpoint` is used to save GPU memory. Please refer to [this page](https://pytorch.org/docs/stable/checkpoint.html) for more details.


### Apex (optional):
Following [Swin Transformer for Object Detection](https://github.com/SwinTransformer/Swin-Transformer-Object-Detection), we use apex for mixed precision training by default. To install apex, run:
```
git clone https://github.com/NVIDIA/apex
cd apex
pip install -v --disable-pip-version-check --no-cache-dir --global-option="--cpp_ext" --global-option="--cuda_ext" ./
```
<!-- If you would like to disable apex, modify the type of runner as `EpochBasedRunner` and comment out the following code block in the [configuration files](configs/swin):
```
# do not use mmdet version fp16
fp16 = None
optimizer_config = dict(
    type="DistOptimizerHook",
    update_interval=1,
    grad_clip=None,
    coalesce=True,
    bucket_size_mb=-1,
    use_fp16=True,
)
``` -->

## Citation
If you use our code/model, please consider to cite our paper [CBNetV2: A Novel Composite Backbone Network Architecture for Object Detection]().
```
@article{liu2021Swin,
  title={Swin Transformer: Hierarchical Vision Transformer using Shifted Windows},
  author={Liu, Ze and Lin, Yutong and Cao, Yue and Hu, Han and Wei, Yixuan and Zhang, Zheng and Lin, Stephen and Guo, Baining},
  journal={arXiv preprint arXiv:2103.14030},
  year={2021}
}
```

## License
The project is only free for academic research purposes, but needs authorization for commerce. For commerce permission, please contact wyt@pku.edu.cn.


## Other Links
> **Original CBNet**: See [CBNet: A Novel Composite Backbone Network Architecture for Object Detection](https://github.com/VDIGPKU/CBNet).

> **SWA**: See [SWA Object Detection](https://github.com/hyz-xmaster/swa_object_detection)
