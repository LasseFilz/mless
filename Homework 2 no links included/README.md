Solution to homework 2, no google drive links included, will need to be added again for it to run smoothly. But the solutions can be seen and evalutated without running anything of course, as plots are included, as well as the data files needed for plotting.

Suggested order of running the notebooks:

1. Add Google Drive Links

2. Notebook 1, second half, download multivariate data

3. Notebook 3-9 in order, train different models and plot results at the end

!IMPORTANT! all private data download links have been removed, and as such the program does not run right now. The links need to be readded for it to run smoothly.

# Timeseries analysis and forecasting based on TOAR data

The [Tropospheric Ozone Assessment Report (TOAR)](https://igacproject.org/activities/TOAR) is an international research activity to provide globally consistent information on the distribution and trends of the air pollutant ozone in the lower part of the atmosphere. Ozone impacts human health, vegetation, and climate, and TOAR provides the data and analyses to quantify the damage caused by ozone.

As the central data service, the [Jülich Supercomputing Centre](https://www.fz-juelich.de/en/ias/jsc) developed and operates the [TOAR Data Infrastructure](https://toar-data.fz-juelich.de/), which stores more than 420,000 time series of ozone and related chemical and meteorological variables. The TOAR data services use a REST API to allow users the download and analysis of custom-tailored datasets. Here, we will make use of this API to obtain and preprocess a couple of exemplary timeseries, which we then use as input data to various machine learning models to demonstrate various aspects around forecasting and interpolation.

The notebooks in this folder are structured as follows:
* 1_Download_Preprocess_data.ipynb: in this notebook, data are downloaded from the TOAR data infrastructure and repackaged so that it can be easily used in the machine learning models
* 2_Data_Analysis.ipynb: here, some visualisations and statistical analyses are demonstrated to gain insights into the data and inform decisions on how the data should be trated in the machine learning workflow
* 3_AutoRegressive_Models.ipynb: this notebook implements a classical statistical technique to establish a baseline against which the ML models can be compared
* 4_MLP.ipynb: here we  build a multilayer perceptron model for timeseries forecasting (**how about RNN?**)
* 5_LSTM.ipynb: this notebook demonstrates a more refined ML architecture for timeseries analysis and forecasting 
* 6_PatchTST.ipynb: finally, we demonstrate the use of a modern, transformer-based architecture for timeseries forecasting
* 7_MLP_multi.ipynb: using both ozone and temp to predict ozone, MLP
* 8_MLP_multi_including_future_temp.ipynb: using both ozone and FUTURE temp to predict ozone, MLP
* 9_multi_model_plotting.ipynb: plot all results in various plots, for comparison

Authors: Sindhu Vasireddy and Martin Schultz, Jülich, May 2025
Co-Author: Lasse Filz, July 2025
