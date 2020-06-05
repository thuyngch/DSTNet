# DSTNet: Unifying Detection, Segmentation, and Tracking via Self-Supervised and Semi-Supervised Learning
Rank 5th in 2D-Tracking and Rank 10th in 2D-Detection, Waymo Open Dataset Challenge 2020

Preprint link: [Dropbox](https://www.dropbox.com/s/zwij9kudu2edrep/cvprw2020_waymo_dstnet.pdf?dl=0)


## Abstract
We present a solution that unifies three fundamental tasks for autonomous driving visual system, which are Detection (D), Segmentation (S), and Tracking (T). Our method, named DSTNet, adopts the simple framework RetinaNet as the base-line, while incorporates several SOTA methods, such as Adaptive Training Sample Selection (ATSS) for detection, ResNeSt backbone, Scale-Equalizing Pyramid Convolution (SEPC), RetinaMask for instance segmentation, and MaskTrack-RCNN for tracking. Our novel contribution is that we combine the COCO and Waymo Open Dataset to perform semi-supervised segmentation training. In addition, we propose the Out-Of-Distribution (OOD) detection technique, where the non-overlapped object categories between Waymo and COCO dataset are treated as unknown classes and trained in a self-supervised manner. Combining these multi-task learning for training and test-time-augmentation (TTA) during inference, our single model, which is trained only by 1 epoch, obtains 43.83/38.01 MOTA L1/L2 and 69.91/63.08 mAP L1/L2 for the 2D Tracking and 2D Detection task of the [Waymo Open Dataset challenge 2020](https://waymo.com/open/challenges), respectively.


## Joint Detection-Segmentation-Tracking demo

![Alt Text](demo/demo1.gif)
![Alt Text](demo/demo2.gif)
![Alt Text](demo/demo3.gif)


## Citation
```
@article{thuync2020dstnet,
  title   = {DSTNet: Unifying Detection, Segmentation, and Tracking via Self-Supervised and Semi-Supervised Learning},
  author  = {Nguyen, Thuy C and Vo, Anh H. and Nguyen, Chuong H. and and Masayuki, Yamazaki},
  journal = {https://github.com/thuyngch/DSTNet},
  year={2020}
}
```
