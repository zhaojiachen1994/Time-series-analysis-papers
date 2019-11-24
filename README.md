# Time series analysis
About time series anomaly detection, prediction
About recurrent neural network, LSTM

## [Table of Contents]()
- [Time series analysis](#Time-series-analysis)
  - [Introductions](#Introduction)
  - [Papers](./papers.md)
  - [Code and repositories](#code-and-repositories)
  - [Datasets and resources](#datasets-and-resources)
  - [其他资源(知乎 教程)](#other-resources)


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



