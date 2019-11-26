# Papers

## [Table of Contents]()
- [Important Papers](#Papers)
  - [Surveys](#survey)
  - [Deep learning and time series](#Deep-learning-and-time-series)
    - [Classification](#Classification)
    - [Segmentation](#Segmentation)
    - [Abnormaly detection](#abnoramly-detection)
    - [Prediction](#prediction) 
  - [SAX representation](#SAX-representation)
  - [Traditional methods on time series](#traditional-methods-on-time-series)
  - [Hot topic with time series](#Hot topic with time series)
  - [Applications](#applications)
  
  
## Surveys


## Deep learning and time series

### Classification

### Segmentation

### Abnormaly detection
- 20191119 `JICAI2019` [Outlier Detection for Time Series with Recurrent Autoencoder Ensembles](https://1drv.ms/b/s!AhuOc8yHadNigcx7SHAmtVaSnLADZQ?e=k6HkSP) [[`Code`](https://github.com/tungk/OED)][*`Abnormaly detection`*]
  - the first proposeal for using recurrent neural network autoencoder ensembles for outlier detection for time series.
  - autoencoder ensembles: 每个encoder随机缺少权重连接，最后在集成多个encoder,避免过拟合。
  - sparsely-connecected RNNs: 随机连接当前时刻之前的几步，再进行集成。

### Prediction
- 20191120 `arXiv2018` [Reveisiting the Hierarchical Multiscale LSTM](https://1drv.ms/b/s!AhuOc8yHadNigcNt-FRl351gG2L37A?e=iWHLgX)[[`Code`](https://github.com/lucaslingle/hm_lstm)][*`Prediction`*]
  - 复现了2016年的论文[Hierarchical multiscale lstm](https://arxiv.org/pdf/1609.01704.pdf), 没有达到预期的效果。
  - Hierarchical multiscale lstm建立了多层的lstm, 层与层之间的状态有相互连接。

## SAX representation
- 20191124 `ICDM2013` [SAX-VSM Interpretable Time Series Classification Using SAX and Vector Space Model](https://1drv.ms/b/s!AhuOc8yHadNigcx45rWhHwQ-h7zO6w?e=vwfYlS) [[`Official code`](https://github.com/jMotif/sax-vsm_classic)]
  - SAX对时间序列进行离散字符表示，用字符串特征的频率来表示每个类别的特征。(SAX+词袋)
  - 词袋中item的频率表示了分类中的重要性，就是Interpretable.

## Traditional methods on time series
- 20191124 `arXiv2012` [Detecting Change-Points in Time Series by Maximum Mean Discrepancy of Ordinal Pattern Distributions](https://1drv.ms/b/s!AhuOc8yHadNigcx3h7VfHuFZuwdyXg?e=Sb4I4x)
  - Oridinal Paatern distribution 描述了一小段子序列中各个数据的大小顺序 (represents the order relations among successive values of a time series)
  - 然后用MMD距离进行two-sample test, 从而判断是否存在change point.

## Hot topic with time series

## Applications
