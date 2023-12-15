# time series forcasting - Machine Learning Task
## Nested CV: Time Series Cross Validation with Time Series Model
## Main Objectives are:
1. Implement the nested time series cross validation strategy for grouped forecasting.
    a. User should provide the dataset, time column and the number of folds to generate
    b. For the given dataset, we will use "day" as a single time unit. This means you can split the data at day level

2. Write you code in sci-kit learn format. Refer to the KFold CV for inspiration. The class should work on pandas dataframes and a datetime column name.

3. Test your code with some samples.

4. Build a time series model on the dataset above and evaluate it using your cross validation method. Submit the notebook illustrating the model development.

5. Submit the code, test samples and any other recorded observations

- This repository contains a Python script for implementing Nested Time Series Cross Validation and building a Time Series Model using scikit-learn. 
- The script is designed to handle time series data and includes an example with synthetic data.

## Requirements

Make sure you have the following packages installed:

- pandas
- numpy
- scikit-learn

You can install them using the following command:

## Code Overview
- The script starts by loading a dataset (train.csv) using pandas.
- NaN values are checked and dropped if necessary.
- Numerical and categorical features are preprocessed.
- The NestedTimeSeriesCV class is defined to implement Nested Time Series Cross Validation.
- The script then uses scikit-learn's TimeSeriesSplit and the custom NestedTimeSeriesCV for cross-validation.
- A basic time series model is built using linear regression as an example.
- Model evaluation metrics (Mean Squared Error and R2 Score) are printed for each fold.

## Results
The script produces the following results:
- Mean Squared Error: 0.01689874204369336, 	 R2 score: 0.41918182130707327
- Mean Squared Error: 1.052695859362339e+19, 	 R2 score: -8.796070382076076e+20
- Mean Squared Error: 0.009157127610516944, 	 R2 score: 0.48934048480704373
- Mean Squared Error: 4.8646400286164386e+19, 	 R2 score: -3.1562575448262333e+21
- Mean Squared Error: 0.007401469497247631, 	 R2 score: 0.5071133430049282
- Mean Squared Error: 0.00722765431485135, 	 R2 score: 0.5853993985595023
- Mean Squared Error: 0.010342423177400948, 	 R2 score: 0.35644495408004706
- Mean Squared Error: 0.006864767351588903, 	 R2 score: 0.5615341422826196
- Mean Squared Error: 0.006918973402801112, 	 R2 score: 0.5246228088121612

