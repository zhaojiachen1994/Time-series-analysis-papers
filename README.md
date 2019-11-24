# Time series analysis
About time series anomaly detection, prediction
About recurrent neural network, LSTM

## [Table of Contents]()
- [Time series analysis](#Time-series-analysis)
  - [Introductions](#Introduction)
  - [Papers](#Papers)
  - [Code and repositories](#code-and-repositories)
  - [Datasets and resources](#datasets-and-resources)
  - [其他资源(知乎 教程)](#)


## Introductions

## Important Papers
- 20191119 `JICAI2019` [Outlier Detection for Time Series with Recurrent Autoencoder Ensembles](https://www.ijcai.org/proceedings/2019/0378.pdf) [[`Code`](https://github.com/tungk/OED)]
  - the first proposeal for using recurrent neural network autoencoder ensembles for outlier detection for time series.
  - autoencoder ensembles: 每个encoder随机缺少权重连接，最后在集成多个encoder,避免过拟合。
  - sparsely-connecected RNNs: 随机连接当前时刻之前的几步，再进行集成。
 
- 20191120 `arXiv2018` [Reveisiting the Hierarchical Multiscale LSTM](https://arxiv.org/abs/1807.03595)[[`code`](https://github.com/lucaslingle/hm_lstm)]
  - 复现了2016年的论文[Hierarchical multiscale lstm](https://arxiv.org/pdf/1609.01704.pdf), 没有达到预期的效果。
  - Hierarchical multiscale lstm建立了多层的lstm, 层与层之间的状态有相互连接。
  
## Code and Repositories
- [ruptures](https://ctruong.perso.math.cnrs.fr/ruptures-docs/build/html/index.html): 一个change point detection的基础python工具包，包括基础的CPD算法，仿真信号，衡量方法。

## Datasets and resources



