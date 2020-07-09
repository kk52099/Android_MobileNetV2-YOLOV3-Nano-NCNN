# MobileNetV2-YOLOv3-Nano NCNN Implementation

This repo provides C++ implementation of [MobileNetV2-YOLOv3-Nano model](https://github.com/dog-qiuqiu/MobileNetv2-YOLOV3) using
Tencent's NCNN framework.

# Notes

Currently NCNN does not support Slice operations with steps, therefore I removed the Slice operation
and replaced the input with a downscaled image and stacked it to match the channel number. This
may slightly reduce the accuracy.

# Screenshot 

![](imgs/screenshot.png)

# Credits 
* [NCNN by Tencent](https://github.com/tencent/ncnn) 
