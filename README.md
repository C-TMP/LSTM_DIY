# NLP-2021 大作业

## 说明

Build an LSTM similar to Pytorch's LSTM by hand 

本项目展示了如何用Pytorch自带的基础类来逐步实现LSTM，模型均在LSTM_DIY里面。LSTMLM.py是主要运行文件。可用LSTM_DIY或官方的nn.LSTM来实例化LSTMLM.py里的TextLSTM里的self.LSTM类查看运行效果，然后运行LSTMLM.py，即可开始训练，训练结束后会显示验证效果。

## 环境

Python 3.8.5

Pytorch 1.9.0

## 模型

其中LSTM_DIY的可用模型有

**LSTM_Layer_v0**

最原始的LSTM，仅支持单向，并且只有一层，无优化，方便初学者联合其forward函数中的代码和LSTM公式来学习如何构建LSTM。

**LSTM_Layer_v1**

功能和LSTM_Layer_v0一样，但向前传播过程中把8个矩阵的乘法优化为2个矩阵的乘法，速度大大提升。

**LSTM_Layer_bi**

在LSTM_Layer_v1的基础上添加了支持双向LSTM的功能。

**LSTM_bi**

在LSTM_Layer_bi的基础上添加了多层LSTM的功能，参数为num_layers。功能和Pytorch的LSTM接近，性能上略有差别。

## 更多信息

详见该大作业对应的报告。
