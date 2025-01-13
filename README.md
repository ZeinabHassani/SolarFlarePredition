# عنوان پروژه

توضیحات پروژه...

---

توضیحات بیشتر...



# SolarFlarePredition
The "Solar Flare Prediction" is a repository for Solar flare  prediction using LSTM and DLSTM with a Sliding window.
This work applies the  Long Short-Term Memory (LSTM) and Deep Decomposition-LSTM (DLSTM) networks on the sliding window (peak flux and within time) to predict the occurrence of solar flares. 

 # Keywords
Solar flare, Imbalance data, Resampling, LSTM, and Decomposition.

# Overview
The project includes the following:
---
Preprocessing: Smoothing, Oversampling Sliding window, and Normalization.
Prediction Solar flare: LSTM and DLSTM networks.

# DataSet
The dataset includes a list of solar flare events from 2003 to 2023 that were obtained  from x-ray GOES data(https://doi.org/10.5281/zenodo.10560188). 

# Results
<img src="https://github.com/ZeinabHassani/SolarFlarePredition/blob/main/Results/roc_0_0_2f_30_LSTM .png" width="400" />
ROC of LSTM without resampling
<img src="https://github.com/ZeinabHassani/SolarFlarePredition/blob/main/Results/roc_0_0_2f_30_D.png" width="400" />
ROC of DLSTM without resampling

<img src="https://github.com/ZeinabHassani/SolarFlarePredition/blob/main/Results/roc_12_0_2f_30_LSTM .png" width="400" />
ROC of LSTM with R=12
<img src="https://github.com/ZeinabHassani/SolarFlarePredition/blob/main/Results/roc_12_0_2f_30_D .png" width="400" />
ROC of DLSTM with R=12
