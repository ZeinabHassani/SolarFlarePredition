# Solar Flare Prediction
The "Solar Flare Prediction" is a repository for Solar flare  prediction using LSTM and DLSTM with a Sliding window.
This work applies the  Long Short-Term Memory (LSTM) and Deep Decomposition-LSTM (DLSTM) networks on the sliding window (peak flux and within time) to predict the occurrence of solar flares. 

 # Keywords
Solar flare, Time series, Imbalance data, Resampling, LSTM, and Decomposition.

# Overview
The project includes the following:

   1. Preprocessing: Smoothing,  and Normalization.

   2. Resampling: Oversampling Sliding Window

   3. Prediction Solar flare: The six models trained for solar flare prediction, each differing in time series format (irregular vs. regular), resampling techniques, and LSTM architecture (LSTM vs. DLSTM). The models utilize a sliding window approach on flare time series and include:
      (1) LSTM applied to irregular time series with various resampling strategies,
      (2) DLSTM on irregular time series with different resampling,
      (3) LSTM on regular time series with a fixed 3-hour interval and resampling,
      (4) DLSTM on regular time series with a 3-hour interval and resampling,
      (5) LSTM on regular time series incorporating resampling and ensemble learning,
      (6) DLSTM on regular time series with resampling and ensemble learning.


# DataSet
The dataset includes a list of solar flare events from 2003 to 2023 that were obtained  from x-ray GOES data(https://doi.org/10.5281/zenodo.10560188). 
this work employs peak flux and waiting time of flares for the prediction of Solar flares

# Results
Our results include 1) LSTM and DLSTM models without resampling and 2) LSTM and DLSTM models with oversampling  R=12, and size window=24.

<img src="https://github.com/ZeinabHassani/SolarFlarePredition/blob/main/Results/roc_0_0_2f_30_LSTM .png" width="400" />  <img src="https://github.com/ZeinabHassani/SolarFlarePredition/blob/main/Results/roc_0_0_2f_30_D.png" width="400" />

ROC of LSTM and DLSTM without resampling 

<img src="https://github.com/ZeinabHassani/SolarFlarePredition/blob/main/Results/roc_12_0_2f_30_LSTM .png" width="400" />  <img src="https://github.com/ZeinabHassani/SolarFlarePredition/blob/main/Results/roc_12_0_2f_30_D .png" width="400" />

ROC of LSTM  and DLSTM  with R=12   

# Authors
[Zeinab Hassani](https://scholar.google.com/citations?user=tDYkBZMAAAAJ&hl=en), [Davud Mohammadpur](https://scholar.google.com/citations?user=f_JH18oAAAAJ&hl=en), and [Hossein Safari](https://scholar.google.com/citations?user=nCc1FV8AAAAJ&hl=en)


