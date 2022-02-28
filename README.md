# deep_learning_with_pytorch
 自己学习Pytorch时构建的一些网络和模板

## Pytorch模板
主要是把Pytorch开发过程中一些常见操作框架化，便于自己的快速开发，目前已经实现对于数据集、model模型、TensorBoard、常用可视化工具等一些的封装，用来开发一些基础网络可以非常快速做验证。
- 模板地址：[Github](https://github.com/ldylab/deep_learning_with_pytorch/tree/main/pytorch_basic_structure)
- brief introduce：[模板比较详细的介绍](https://ldylab.cc/2022/02/28/Pytorch_template/)

## 基于Pytorch的相关基础模型的开发
主要是自己在学习网络过程中阅读论文所复现的一些模型，个人目前主要还是比较集中在目标检测识别这一方向中，后续会继续「读论文-自己造轮子-复现相关方向论文」，希望可以进一步熟悉Pytorch框架，并能够用通俗易懂的语言描述论文的思想框架并将其思想可视化，并最终能提出自己的一些东西，目前已经完成基于CiFar10数据集的分类网络，后续会继续完善笔记和其他模型：
- LeNet：[代码](https://github.com/ldylab/deep_learning_with_pytorch/blob/main/pytorch_basic_structure/model/lenet5/lenet_5_model.py)；
- AlexNet：[代码](https://github.com/ldylab/deep_learning_with_pytorch/blob/main/pytorch_basic_structure/model/alexnet/alexnet_model.py)；
- VGGNet：[代码](https://github.com/ldylab/deep_learning_with_pytorch/blob/main/pytorch_basic_structure/model/vggnet/vggnet16.py)；
- ResNet：[代码](https://github.com/ldylab/deep_learning_with_pytorch/blob/main/pytorch_basic_structure/model/resnet/resnet34_model.py)，[笔记：ResNet可视化过程](https://ldylab.cc/2022/02/28/ResNet34_Visual/)；
- DenseNet：[代码](https://github.com/ldylab/deep_learning_with_pytorch/blob/main/pytorch_basic_structure/model/densenet/densenet_model.py)
- CotNet：[代码](https://github.com/ldylab/deep_learning_with_pytorch/blob/main/pytorch_basic_structure/model/cotnet/cotnet_model.py)；

项目所使用的环境为：
- CUDA 10.0/10.2；
- python 3.7.10；
- Pytorch 1.2~1.7；
  
在项目代码中，`options.py`中选择模型、数据集，并设置参数（Batch_size、epoch等），并运行：
```python
python train.py # 训练模型
python eval.py # 测试模型，并其结果可视化
```
即可。
