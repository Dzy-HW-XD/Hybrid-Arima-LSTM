# 基于Hybrid ARIMA-Attention based LSTM S&P500股票预测
自2003年Zhang(https://www.sciencedirect.com/science/article/abs/pii/S0925231201007020) 先生将基于传统统计的ARIMA与神经网络结合以来，人们开始思考线性模型与非线性模型结合的可能性。此次实验，得益于近年深度学习的飞速发展，更优秀性能的非线性模型的出现让我们能够站在巨人的肩膀上继续前行，本次实验，我们将对Hybrid-Arima-attention based LSTM与其他prue模型(Prue ARIMA,Prue LSTM, Prue LSTM-Attention)在时序预测任务上的表现进行评估，对比，总结。


## Abstract

Forecasting task based on time-sequential data is
a hot topic in various domains such as, finance, urban management, astronomical forecasting. Very
recently, the superiority of deep learning has
gained increasing attention in forecasting task.
Long Short-Term Memory(LSTM), as a recurrent model naturally has the ability to handle
time series forecasting task and present a state of
art performance. In this report, we treat LSTM
as the baseline model and improved it through
two ways: data enhancement and model structure
improvement. The idea of data enhancement is inspired from (Zhang, 2003), which establish a superior hybrid model composed of Autoregressive
integrated moving average(ARIMA) and LSTM.
The idea of model structure improvement is inspired from (Qin et al., 2017b) which import the
attention mechanism. We will apply them to SP
500 dataset an the performance will be evaluated
by comparing with baseline.

## 数据选择：

 | 数据集名称  | 数据大小 | 训练集 | 测试集 |
 | ------------| -------- | ------ | ---- |
 | SP500 Index | 6755 | 6000 | 755 |
 | AAL  | 1259 | 1000 | 259 |
 | ABC  | 1259 | 1000 | 259 |

### Results Table 
![resulttable](https://github.com/Dzy-HW-XD/Hybrid-Arima-LSTM/blob/main/results_tables.jpg)

### Pure ARIMA 
![sp500](https://github.com/Dzy-HW-XD/Hybrid-Arima-LSTM/raw/main/results_figures/pure_ARIMA_sp500_overall.png) 
![AAL](https://github.com/Dzy-HW-XD/Hybrid-Arima-LSTM/raw/main/results_figures/pure_ARIMA_AAL_overall.png) 
![ABC](https://github.com/Dzy-HW-XD/Hybrid-Arima-LSTM/raw/main/results_figures/pure_ARIMA_ABC_overall.png) 

### Pure LSTM
![sp500](https://github.com/Dzy-HW-XD/Hybrid-Arima-LSTM/blob/main/results_figures/pure_LSTM_sp500_overall.png) 
![AAL](https://github.com/Dzy-HW-XD/Hybrid-Arima-LSTM/raw/main/results_figures/pure_LSTM_AAL_overall.png) 
![ABC](https://github.com/Dzy-HW-XD/Hybrid-Arima-LSTM/raw/main/results_figures/pure_LSTM_ABC_overall.png) 

### Hybrid
![sp500](https://github.com/Dzy-HW-XD/Hybrid-Arima-LSTM/blob/main/results_figures/hybird_sp500_overall.png) 
![AAL](https://github.com/Dzy-HW-XD/Hybrid-Arima-LSTM/blob/main/results_figures/hybird_AAL_overall.png) 
![ABC](https://github.com/Dzy-HW-XD/Hybrid-Arima-LSTM/blob/main/results_figures/hybird_ABC_overall.png) 


