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
- 20191119 `JICAI2019` [Outlier Detection for Time Series with Recurrent Autoencoder Ensembles](https://www.jianguoyun.com/p/DUG3T8cQ5sn0Bxiyk6EC) [[`Code`](https://github.com/tungk/OED)]
  - the first proposeal for using recurrent neural network autoencoder ensembles for outlier detection for time series.
  - autoencoder ensembles: 每个encoder随机缺少权重连接，最后在集成多个encoder,避免过拟合。
  - sparsely-connecected RNNs: 随机连接当前时刻之前的几步，再进行集成。
  
## Code and Repositories
- [ruptures](https://ctruong.perso.math.cnrs.fr/ruptures-docs/build/html/index.html): 一个change point detection的基础python工具包，包括基础的CPD算法，仿真信号，衡量方法。

- 

## Datasets and resources


## Other resources



