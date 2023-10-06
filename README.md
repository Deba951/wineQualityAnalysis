# wineQualityAnalysis

![peakpx](https://github.com/Deba951/wineQualityAnalysis/assets/83878346/6dbe16ac-9693-4ccb-a2ee-02f604968ea5)


We will be predicting the quality of wine on the basis of some given features. 
We will use the wine quality dataset available on the Internet for free. This dataset has the fundamental features which are responsible for affecting the quality of the wine.

## Importing libraries and Dataset:
```
Pandas - is a useful library in data handling.
Numpy - The library is used for working with arrays.
Seaborn/Matplotlib is used for data visualisation purposes.
Sklearn – This module contains multiple libraries having pre-implemented functions to perform tasks from data preprocessing to model development and evaluation.
XGBoost – This contains the eXtreme Gradient Boosting machine learning algorithm which is one of the algorithms that helps us to achieve high accuracy on predictions
```

## The quality of a wine is determined by :

```
Type
Fixed acidity
Volatile acidity
Citric Acid
Residual Sugar
Chlorides
Free Sulfur dioxide
Total Sulfur dioxide
Density
pH
Sulphates
Alcohol
Quality
```


## Objective

The objectives of this project are as follows:

```
To experiment with different classification methods to see which yields the highest accuracy
To determine which features are the most indicative of a good quality wine
```

## Steps included in this project:

1. **Import Libraries:**
   - Import necessary Python libraries, including NumPy, pandas, matplotlib, Seaborn, and sci-kit-learn modules.

2. **Load Data:**
   - Load a dataset named 'winequality.csv' into a pandas DataFrame (`df`).
   - Print the first few rows of the DataFrame to inspect the data.

3. **Data Exploration:**
   - Use `df.info()` to display information about the DataFrame, including data types and missing values.
   - Use `df.describe().T` to generate summary statistics for the numeric columns.
   - Check for missing values using `df.isnull().sum()` and fill missing values with column means.

4. **Data Visualization:**
   - Plot histograms for each numeric feature using `df.hist()`.
   - Create a bar plot to visualize the relationship between 'quality' and 'alcohol' content.

5. **Correlation Analysis:**
   - Calculate the correlation matrix of numeric features using `numeric_df.corr()`.
   - Visualize the correlation matrix with a heatmap, highlighting correlations above 0.7.

6. **Feature Engineering:**
   - Remove the 'total sulfur dioxide' column from the DataFrame using `df.drop()`.
   - Create a new binary column 'best quality' where 1 indicates quality greater than 5 and 0 otherwise.
   - Replace 'white' and 'red' values in the DataFrame with 1 and 0, respectively.

7. **Data Splitting:**
   - Split the dataset into training and testing sets using `train_test_split()` with an 80-20 split ratio.
   - Normalize the features using Min-Max scaling with `MinMaxScaler()`.

8. **Model Building:**
   - Create a list of machine learning models including Logistic Regression, XGBoost, and Support Vector Classifier (SVC).
   - Train each model on the training data and evaluate their performance on both training and testing data.
   - Print training and validation accuracy for each model.

9. **Confusion Matrix:**
   - Plot the confusion matrix for the XGBoost model using `metrics.plot_confusion_matrix()`.

10. **Classification Report:**
    - Print a classification report for the XGBoost model, including metrics like precision, recall, and F1-score.

CHEERS!
![kelsey-knight-udj2tD3WKsY-unsplash](https://github.com/Deba951/wineQualityAnalysis/assets/83878346/beadaafd-04a2-4776-b132-bd8da417984e)

Feel free to drop a star if you like it.
