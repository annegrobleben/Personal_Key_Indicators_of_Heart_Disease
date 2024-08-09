This notebook is based on an assignment done as part of a Master in Data Science & AI at Nuclio Digital School, it shows how to create a binary classification model that predicts the likelihood of someone having a heart disease based on their answers in a survey.

The assignment is split into three main parts: data understanding, data cleaning and model buidling. When building and evaluating the model special attention is paid to the Recall score, the model's ability to detect true positives as such. We begin with four different models: a decision tree, a logistic regression, a random forest and a gradient boosting classifier. The logistic regression and the gradient boosting classifier perform significantly better than the other two models, which is why only those two are optimized further.

1) Data understanding
       1.1 Import dataset and data dictionary
   - 1.2 Check for duplicates
   1.3 Check datatypes and correct them if necessary
   1.4 Descriptive statistics
   1.5 Detection of null values
   1.6 Distribution of target values
   1.7 Check for outliers
   1.8 Visualization of numeric distributions and error detection
   1.9 Visualization of categorical distributions
   
3) Data cleaning
   2.1 Handling outliers
   2.2 Imputation of null values and Encoding

4) Modelling
   3.1 Get a first idea of feature correlations with target variable
   3.2 Decision Tree
   3.3 Logistic Regression
   3.4 Random Forest
   3.5 Gradient Boosting Classifier
   3.6 Dimensionality reduction
   3.7 Resampling
   3.8 Reverse outlier treatment in Age column
   3.9 Conclusion

This notebook was created in Google Colab. In order to run it in Google Colab the attached csv-files "heart_disease_data.csv" and "data_dictionary" need to be added to "MyDrive" in Google drive in a folder named "SupervisedMachineLearningn" so that the code cell 4 and 5 can be run properly. In case that this notebook is run in an application that is different from Google Colab part "1.1 Import dataet and data dictionary" needs to be adjusted beforehand.
