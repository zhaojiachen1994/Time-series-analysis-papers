# Time series analysis
About time series anomaly detection, prediction
About recurrent neural network, LSTM

## [Table of Contents]()
- [Time series analysis](#Time-series-analysis)
  - [Introductions](#Introduction)
  - [Papers](./papers.md)
  - [Code and repositories](#code-and-repositories)
  - [Datasets and resources](#datasets-and-resources)
  - [其他资源(知乎 教程)](#other-resources):some interesting cases
  - [Documents about wearable computing](#Documents about wearable computing)


## Introductions

## Important Papers
- 20191119 `JICAI2019` [Outlier Detection for Time Series with Recurrent Autoencoder Ensembles](https://www.ijcai.org/proceedings/2019/0378.pdf) [[`Code`](https://github.com/tungk/OED)]
  - the first proposeal for using recurrent neural network autoencoder ensembles for outlier detection for time series.
  - autoencoder ensembles: 每个encoder随机缺少权重连接，最后在集成多个encoder,避免过拟合。
  - sparsely-connecected RNNs: 随机连接当前时刻之前的几步，再进行集成。
  
- 20191124 `CVPR2018` [Independently Recurrent Neural Network (IndRNN): Building A Longer and Deeper RNN](https://arxiv.org/abs/1803.04831) [[`Comment`](https://www.jianguoyun.com/p/Dfw2rYoQ5sn0BxjIk6EC)] [[`code`](https://github.com/Sunnydreamrain/IndRNN_pytorch)]
  - 对普通RNN的一种简化，认为序列的各个维度之间相互独立，原本正向传递时的矩阵乘法变为向量乘法。
  - 记忆长度更长，克服梯度消失问题。
  - 深度IndRNN投稿到CVPR2019: [Deep Independently Recurrent Neural Network (IndRNN)](https://arxiv.org/pdf/1910.06251.pdf)



## Code and Repositories
- [ruptures](https://ctruong.perso.math.cnrs.fr/ruptures-docs/build/html/index.html): 一个change point detection的基础python工具包，包括基础的CPD算法，仿真信号，衡量方法。

- [seglearn](https://dmbee.github.io/seglearn/): 一个对时间序列分段、提取特征的python工具包





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

