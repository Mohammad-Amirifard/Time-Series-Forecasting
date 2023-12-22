
# Rpository Structure:
```
- 📦 Time Series
  |- 📄 README.md        #this file
  |- 📂 data             #local data folder
  |- 📂 Notebooks        #Here you can see a Main.ipynb which the main file. You can run it on Google Colab
  |- 📂 Submissions      #Here you can see a zip file which is appropraite to upload in Coda Lab
  |- 📂 Report           #Here you can see our report.
```


# Project Detail

**Problem**: Time Series Forecasting

**Goal**: The task is to develop a forecasting model that is able to predict several uncorrelated time series. The prerequisite is that the model exhibits generalisation capabilities in the forecasting domain, allowing it to transcend the constraints of specific time domains. This requires a model that, while specialised in forecasting, is not limited to predicting in a single or predefined time context.

# Dataset Detail:

**Time series length**: the length of the time series in the training dataset is variable. To simplify the portability of the dataset, we padded with zeros the sequences to the maximum length of 2776. Thus, the dataset is provided in a compact form as a Nx2776 array. We provide an additional 'valid_periods.npy' file containing the information to recover the original time series without the padding

**File Format**: npy

**Categories**: the provided time series are composed by sequences collected from 6 different sources. We further provide additional information about the category of each time series.

**Datas Structure**: Single folder containing the following files:

'training_data.npy': it contains a numpy array of shape (48000, 2776). 48000 time series of length 2776.
'valid_periods.npy': it contains a numpy array of type (48000, 2) containing for each of the time series the start and end index of the current series, i.e. the part without padding.
'categories.npy': it contains a numpy array of shape (48000,), containing for each of the time series the code of its category. The possible categories are in {'A', 'B', 'C', 'D', 'E', 'F'}.
IMPORTANT: This is a dataset consisting of monovariate time series, i.e. composed of a single feature, belonging to six different domains. The time series of each domain are not to be understood as closely related to each other, but only as collected from similar data sources. What is required of you is therefore to build a model that is capable of generalising sufficiently to predict the future samples of the 60 time series of the test set. To download **datset**, click on the link below: link and for **github repositoy** please click on this: Link



