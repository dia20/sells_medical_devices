# Sells Medical Devices
You are provided with customer data from a company that sells medical devices. The business owner has not collected any demographic data about the customers. However, he is interested in the similarities between customers and the relationships between his customer data. You provide him with some guidance using your data mining skills
# Modelling the Random Forest relationship between Customers and Customer Satisfactions

The contents of this project are divided into following topics which are listed as follows:-

# Table of Contents: 

1. Task Description
2. Data Description
3. Data Preparation 
4. Data Exploration
5. Data Visualization
6. Preprocessing
7. Feature generation and transformation
8. Model development 
9. Results and Conclusion 


# 1. Task Description

For the purposes of this project, we will create a random forest algorithm to examine customer information from a business that sells medical products. Our objective is to use data mining and business intelligence techniques to give the business owner insights into the links between his customer data and the similarities amongst his customers.

# 2. Data Description

Customer information from a business that sells medical devices makes up the data. The customer ID, business year of operation, number of sales calls made to that customer, number of targeted emails sent to that customer, number of sales to that customer, and customer satisfaction index are all included in the dataset. There are no client demographics in the data.

# 3. Data Preparation 

The data's datatype is one of the first things to note. There are no empty values in the data. There are no outliers in the data, which has a specified range.  There is no need to transform the data to dummy variables because it just contains numerical values. The data must be normalized because the year column in the data contains distances for the data. 

# 4. Data Exploration
In order to comprehend the data's attributes and qualities better, we looked into it. To view introductory statistics and information on the data, we utilized pandas methods like describe() and info(). To observe the distributions and correlations between the various variables, we also used visualizations including histograms, scatter plots, and box plots.

# 5. Data Visualization

Principle Component Analysis (PCA)
Bar Chart 
Pie Chart
Histogram
Cluster Method (K-Means)
Correlation
Area Under the Curve (AUC)

# 6. Preprocessing

I select Random Forest as my classification model because it doesn't have a lot of features and isn't very complex. Random forests, also known as random decision forests, are an algorithm model that is used in this assignment to provide answers to all of the business owner's considerations. As an ensemble learning technique for classification, regression, and other problems, random forests build a large number of decision trees during the training phase. The class that the majority of the trees chose is the output of the random forest for classification problems.

# 7. Feature generation and transformation

As necessary, we generated and changed features. To enhance the functionality of our model, we applied techniques like scaling and normalization. To keep the data within the same range, we normalize the year column, which has two decimals. Since we employed the PCA, we also performed the normalization on the entire set of data. 

# 8. Model development

To examine the data, a random forest model was created. To build a model with the required number of trees and other hyperparameters, we used scikit-learn's RandomForestClassifier or RandomForestRegressor.

# 9. Results and Conclusion

Based on information we gather from our clients, the classification system we built is intended to assist us in making crucial business decisions. On the basis of their behavior and preferences, we're specifically employing the algorithm to divide our consumers into one of three groups. 

Unfortunately, the algorithm's accuracy falls short of our expectations. This indicates that the algorithm is not appropriately identifying our consumers as well as we would want. But it's crucial to remember that accuracy is only one of several measures we can use to gauge how well the algorithm is working. 

The size and complexity of the method are two elements that may be contributing to its poor performance.  


## Python libraries
I have Anaconda Python distribution installed on my system. It comes with most of the standard Python libraries I need for this project. The basic Python libraries used in this project are:-
```
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
import matplotlib as mpl
%matplotlib inline
from sklearn.model_selection import cross_val_score
from sklearn.metrics import roc_curve, auc
from sklearn.pipeline import make_pipeline
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.preprocessing import label_binarize
from sklearn.ensemble import RandomForestClassifier
from sklearn.model_selection import StratifiedKFold
import pandas as pd
import numpy as np
```

