# Papers

## [Table of Contents]()
- [Important Papers](#Papers)
  - [Surveys](#survey)
  - Method category
    - [Deep learning and time series](#Deep-learning-and-time-series)
    - [SAX representation](#SAX-representation)
  - Task category
    - [Classification](#Classification)
    - [Segmentation](#Segmentation)
    - [Abnormaly detection](#abnoramly-detection)
    - [Prediction](#prediction)
  - [Application](#application)
  
## Surveys


## Deep learning and time series
- 20191119 `JICAI2019` [Outlier Detection for Time Series with Recurrent Autoencoder Ensembles](https://www.ijcai.org/proceedings/2019/0378.pdf) [[`Code`](https://github.com/tungk/OED)]
  - the first proposeal for using recurrent neural network autoencoder ensembles for outlier detection for time series.
  - autoencoder ensembles: 每个encoder随机缺少权重连接，最后在集成多个encoder,避免过拟合。
  - sparsely-connecected RNNs: 随机连接当前时刻之前的几步，再进行集成。
 
- 20191120 `arXiv2018` [Reveisiting the Hierarchical Multiscale LSTM](https://arxiv.org/abs/1807.03595)[[`Code`](https://github.com/lucaslingle/hm_lstm)]
  - 复现了2016年的论文[Hierarchical multiscale lstm](https://arxiv.org/pdf/1609.01704.pdf), 没有达到预期的效果。
  - Hierarchical multiscale lstm建立了多层的lstm, 层与层之间的状态有相互连接。

## SAX representation
- 20191124 `ICDM2013` [SAX-VSM Interpretable Time Series Classification Using SAX and Vector Space Model](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.715.4227&rep=rep1&type=pdf) [[`Official code`](https://github.com/jMotif/sax-vsm_classic)]
  - SAX对时间序列进行离散字符表示，用字符串特征的频率来表示每个类别的特征。(SAX+词袋)
  - 词袋中item的频率表示了分类中的重要性，就是Interpretable.
  
## Classification


## Segmentation

## Abnormaly detection

## Prediction

## Application
