# Dataset-for-Deal-Banking-Marketing-Campaigns-Using-ML
The data is related to the direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact with the same client was required, to assess if the product (bank term deposit) would be ('yes') or not ('no') subscribed by the customer or not. The data folder contains two datasets:-

1: train.csv: 45,211 rows and 18 columns 

2: test.csv: 4521 rows and 18 columns 

We can see some binary columns(default, housing, loan) that are object types we need to convert into numeric values.

There are categorical columns also, but there are a limited number of choices. They are job, marital, education, contact, month, and poutcome. That also needs to be converted into numerical format.

All feature columns we need to convert into numeric values only then can we feed into the model.

We can convert the yes values to 1, and the no values to 0 for the default column. We will use Label Encoder function for this.

Handling imbalanced dataset

Since the class distribution in the target variable is ~89:11 indicating an imbalanced dataset, we need to resample it. This problem is seen where the no.of observations belonging to one class is significantly lower than those belonging to other classes. The Different Approaches for Handling imbalanced Data are Resampling(apply SMOTE function), Cluster-Based Oversampling. We have a package named “imblearn” which is mostly preferred for solving the Class imbalance problem.

Several machine learning models are used in this dataset, all in the form of arrays, in just one computation.
