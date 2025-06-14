# ss-Assignment-17
In this third practical application assignment, your goal is to compare the performance of the classifiers (k-nearest neighbors, logistic regression, decision trees, and support vector machines) you encountered in this section of the program. You will use a dataset related to the marketing of bank products over the telephone.

I used CRISP-DM to resolve this problem, Steps taken are as follows:

1)	Studied and loaded the data in Pandas dataframe.
2)	Column duration was dropped as per “database creator’s instructions’.
3)	Column emp.var.rate, cons.price.idx, cons.conf.idx, and nr.employed should be dropped as they are correlated to euribor3m.
4)	Renamed column “Y” to “subscribed”.
5)	Renamed “default” to “credit_default”
6)	Listed unique values along with their percentages for all columns in clean_df.
7)	Calculated percentage of null values per column in clean_df.
8)	Since credit_default has 20% unknown It was best to drop it.
9)	Removed rows with "unknown" values. Maximum it will impact 4% of rows.
10)	Plotted  histograms for all values in all columns cleaned dataframe.
11)	After seeing histogram plots, dropeed day of the week column - it is uniformly distributed. Also dropped pdays as it is majorly driven by greater than 999 days. Also dropping month as there should be no relation to deposits with months.
12)	found number of unique values for all object columns.
13)	Used Labelencoder and Hotencoders on non integer and non float columns.
14)	Split data into test and train datasets.
15)	Ran four models and found Logisticregression and KNN to be better than SVM and DecisionTree.
16)	Used Pipline and hyperparameters to check feature engineering. Found both model worked best with degree 1.

Recommendation – For this database first degree Logistic regression should be used. 




