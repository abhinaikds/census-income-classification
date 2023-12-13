#Insights by EDA:
1. There was "?" in "workclass" feature and it was replaced by np.nan and then imputed the most frequent class in place of nan.
2. There was trailing, leading spaces in certain cells and it is removed.
3. Removed Education column since it already had the education-num column which is the same.

Data Preprocessing steps:
1. Separated all categorical and numerical values and applied one hot encoder and standardized numerical values respectively.
2. since the data is not Balanced, RandomOverSampler is used to balance the data.

Model Building and pickling:
Trained cleaned data with required algorithms and found that the Random forest algorithm is giving the best accuracy, the model is then pickled to save locally and then loaded back to use the pickled model to predict the output.
