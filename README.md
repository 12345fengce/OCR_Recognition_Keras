# OCR_Recognition_Keras
## 说明
本代码是基于CRNN的OCR识别写的代码。主要基于keras，代码主要分为两种路线：<br>
一：舍弃RNN结构，单独使用CNN结构。其中CNN使用VGG网络结构完成；<br>
二：采用CNN + RNN + Attention 的结构模式。将Attention带入识别中。

## Data
本文这里使用的数据为360W的数据集。网上都是可以下载到的。具体数据样式如下：

![image](https://github.com/Tian14267/OCR_Recognition_Keras/tree/master/images/data.png)

## Train
数据整理好之后，就是训练环节，直接运行 train_attention_linux.py 代码就可以了。<br>
PS：注意修改相关配置<br>
训练细节如下：<br>

![image](https://github.com/Tian14267/OCR_Recognition_Keras/tree/master/images/train.png)

上图是基于CNN_Only训练的，还没训练完。等完全训练完之后，其识别率能达到98%以上。<br>
注：经过测试发现，添加attention机制后的识别系统，其识别效果要差很多。大概也就90%的正确率
