This notebook is based on an assignment done as part of a Master in Data Science & AI at Nuclio Digital School, it shows how to create a binary classification model hat predicts the likelihood of someone having a heart disease based on their answers in a survey.

The survey responses and the data dictionary are both loaded into a dataframe. In the data understanding stage we check the data for duplicates, investigate the datatypes and correct them if necessary, run descriptive statistics and look at the distribution of the target values as well as null values and outliers.

Then, some univariate visualizations are produced before we present some graphics for each variable against the target variable. In these visualizations some trends can be spotted in the data, for example we see that the distribution of respondents who have ever had a stroke is different among those with a heart disease than for the whole dataset.

Before going into the modelling phase we find an adequate treatment for the outliers and null values. Besides, the categorical variables are encoded using the OneHot and Ordinal encoding methods.

When building and evaluating the model special attention is paid to the Recall score, the model's ability to detect true positives as such. We begin with four different models: a decision tree, a logistic regression, a random forest and a gradient boosting classifier. The logistic regression and the gradient boosting classifier perform significantly better than the other two models, which is why only those two are optimized further.

Dimensionality reduction has no effect on the performance of both models, only with Resampling the performance metrics improve notably. We also try to see if there are any changes if we reverse the outlier treatment previously done in one category, but afterwards the Recall scores of models increase only by less than 1%.

Even though the gradient boosting classifier ends up having the higher test accuracy the logistic regression is considererd the best-performing model as it has the highest Recall score.

This notebook was created in Google Colab. In order to run it in Google Colab the attached csv-files "heart_disease_data.csv" and "data_dictionary" need to be added to "MyDrive" in Google drive in a folder named "SupervisedMachineLearningn" so that the code cell 4 and 5 can be run properly. In case that this notebook is run in an application that is different from Google Colab part "1.1 Import dataet and data dictionary" needs to be adjusted beforehand.
