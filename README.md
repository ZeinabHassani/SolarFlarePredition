# Solar Flare Prediction
The "Solar Flare Prediction" is a repository for Solar flare  prediction using LSTM and DLSTM with a Sliding window.
This work applies the  Long Short-Term Memory (LSTM) and Deep Decomposition-LSTM (DLSTM) networks on the sliding window (peak flux and within time) to predict the occurrence of solar flares. 

 # Keywords
Solar flare, Time series, Imbalance data, Resampling, LSTM, and Decomposition.

# Overview
The project includes the following:

   1. Preprocessing: Smoothing,  and Normalization.

   2. Resampling: Oversampling Sliding Window

   3. Prediction Solar flare: LSTM and DLSTM networks.


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


