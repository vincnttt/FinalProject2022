### 链接
[MMDetection官网](https://mmdetection.readthedocs.io/en/latest/)

[MMDetection开源](https://github.com/open-mmlab/mmdetection)

### 环境配置
```bash
git clone https://github.com/open-mmlab/mmdetection.git
cd mmdetection
pip install -v -e .
```
*上次在电脑上下载有问题[pycocotools wheel]下不了，可以尝试在华为云下载搭配*

如果可以的话，把[custom_faster_rcnn_r50_fpn.py]文件复制到[mmdetection/configs/faster_rcnn/]里面。

然后在目录中[mmdetection/configs/faster_rcnn/]打开cli，运行以下命令进行训练和测试模型
```bash
# training is just one line.
!python tools/train.py configs/faster_rcnn/custom_faster_rcnn_r50_fpn.py
# You can also test the model like this.
!python tools/test.py configs/faster_rcnn/custom_faster_rcnn_r50_fpn.py YOUR_MODEL_PATH --eval bbox
```

### 参考
https://blog.csdn.net/euqlll/article/details/127556989
