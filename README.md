# Solar Flare Prediction
The "Solar Flare Prediction" is a repository for Solar flare prediction using LSTM and DLSTM with a Sliding window and an ensemble algorithm.
This work applies the  Long Short-Term Memory (LSTM) and Deep Decomposition-LSTM (DLSTM) networks on the sliding window to detect temporal quasi-patterns in irregular and regular flare time series from 2003 to 2023 recorded by GOES.

 # Keywords
Solar flare, Time series, Imbalanced data, Resampling, LSTM, and Decomposition.

# Overview
The project includes the following:

   1. **Preprocessing:** Smoothing, Normalization, and Regularization.
    
   2. **Resampling:** Oversampling Sliding Window

   3. **Prediction Solar flare:** The six models trained for solar flare prediction, each differing in time series format (irregular vs. regular), resampling techniques, and LSTM architecture (LSTM vs. DLSTM). The models utilize a sliding window approach on the flare time series, including:
      1) LSTM applied to irregular time series with various resampling strategies,
      2) DLSTM on irregular time series with different resampling,
      3) LSTM on regular time series with a 3-hour interval and resampling,
      4) DLSTM on regular time series with a 3-hour interval and resampling,
      5) LSTM on regular time series incorporating resampling and ensemble learning,
      6) DLSTM on regular time series with resampling and ensemble learning.


# DataSet
The dataset includes a list of solar flare events from 2003 to 2023 that are obtained  from x-ray GOES data(https://doi.org/10.5281/zenodo.10560188). 
This work employs peak fluxes and waiting times of irregular flare time series. Also, the irregular flare time series is regularized  with a 3-hour interval  that contains maximum peak fluxes within each interval.

# Results
Our results include six different models in the irregular(original data) and regular flare without resampling R=0 and with oversampling  R=12, by size window=24.

<img src="https://github.com/ZeinabHassani/SolarFlarePredition/blob/main/Results/ROC_6models_R0.png" width="400" />
ROC of six models without resampling 
<img src="https://github.com/ZeinabHassani/SolarFlarePredition/blob/main/Results/ROC_6models_R12.png" width="400" />
ROC of six models with oversampling  R=12   

# Authors
[Zeinab Hassani](https://scholar.google.com/citations?user=tDYkBZMAAAAJ&hl=en), [Davud Mohammadpur](https://scholar.google.com/citations?user=f_JH18oAAAAJ&hl=en), and [Hossein Safari](https://scholar.google.com/citations?user=nCc1FV8AAAAJ&hl=en)

# Citation
If it is useful, please cite our paper:

  @ARTICLE{Solarflare_2025,
  
     author = {Hassani, Zeinab and Mohammadpur, Davud and Safari, Hossein },
     
     year = {2025},
     
     title = {Solar Flare Prediction Using LSTM and DLSTM with Sliding Window Pattern Recognition},
     
     doi = {https://doi.org/10.3847/1538-4365/addc73}
     
}


