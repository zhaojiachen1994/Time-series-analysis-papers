# Time series analysis
About time series anomaly detection, prediction
About recurrent neural network, LSTM

## [Table of Contents]()
- [Time series analysis](#Time-series-analysis)
  - [Introductions](#Introduction)
  - [Papers](./papers.md)
  - [Code and repositories](#code-and-repositories)
  - [Datasets and resources](#datasets-and-resources)
  - [其他资源(知乎 教程)](#other-resources): some interesting cases


## Introductions

## Important Papers

- 20191212 `TNNLS2019` [Unsupervised Anomaly Detection with LSTM Neural Networks]
(https://1drv.ms/b/s!AhuOc8yHadNigc1WN8NNWnDgedoBXw?e=xXhzNP) [`code`]
  - 利用LSTM进行编码，利用one class SVM来计算异常分数，综合训练
  - LSTM+OCSVM+quadratic programming training, LSTM+OCSVM+gradient-based training, LSTM+SVDD
  - 数学推导比较好，实验一般
  - [Smooth maximum](https://en.wikipedia.org/wiki/Smooth_maximum)将最大值优化问题近似为可导函数的方法可以参考

- 20191125 `ICLR2018` [Deep Autoencoding Gaussian Mixture Model for Unsupervised Anomaly Detection](https://1drv.ms/b/s!AhuOc8yHadNigcxmXTqsW3LIxzzc6g?e=fCGKDV)[[`code`](https://github.com/danieltan07/dagmm)]
  - 包括一个编码网络和估计网络，同一训练，损失函数包括编码误差和聚类熵。
  - 编码网络输入原始数据，输出restructured error and hidden feature;估计网络进行高斯混合分布概率的估计，概率小的为outlirer.
  
- 20191124 `CVPR2018` [Independently Recurrent Neural Network (IndRNN): Building A Longer and Deeper RNN](https://1drv.ms/b/s!AhuOc8yHadNigcx6xIkuQMNcCixhSQ?e=RVyKyv)[[`code`](https://github.com/Sunnydreamrain/IndRNN_pytorch)]
  - 对普通RNN的一种简化，认为序列的各个维度之间相互独立，原本正向传递时的矩阵乘法变为向量乘法。
  - 记忆长度更长，克服梯度消失问题。
  - 深度IndRNN投稿到CVPR2019: [Deep Independently Recurrent Neural Network (IndRNN)](https://arxiv.org/pdf/1910.06251.pdf)

## Code and Repositories
- [ruptures](https://ctruong.perso.math.cnrs.fr/ruptures-docs/build/html/index.html): 一个change point detection的基础python工具包，包括基础的CPD算法，仿真信号，衡量方法。

- [seglearn](https://dmbee.github.io/seglearn/): 一个对时间序列分段、提取特征的python工具包

- [Downloader for real-world datasets](https://github.com/chickenbestlover/RNN-Time-series-Anomaly-Detection/blob/master/0_download_dataset.py):RNN时间序列异常检测的真实数据下载器。



## Datasets and resources


## Other resources

- Kaggle
  - [利用RNN处理大型时间序列数据，进行地震的预测](https://www.kaggle.com/mayer79/rnn-starter-for-huge-time-series)
- 知乎
  - [一个简短精彩的关于RNN中学习长期依赖的三种机制的概述](https://zhuanlan.zhihu.com/p/34490114)
  - [知乎时间序列分析专栏](https://zhuanlan.zhihu.com/c_1071087593646698496)
  - [RNN中为什么要用tanh,而不是ReLU作为激活函数](https://www.zhihu.com/question/61265076/answer/260492479)
  - [时间序列预测方法总结知乎专栏](https://zhuanlan.zhihu.com/p/67832773)
  
  
- Documents about wearable computing
  - 人机交互百科全书的第二章：[Wearable computing, including concepts and applications(英文)](https://www.interaction-design.org/literature/book/the-encyclopedia-of-human-computer-interaction-2nd-ed/wearable-computing) 

