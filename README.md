# **Data Science for the retail sector**
Data science offers some powerfull techniques to take advantage of the customer data that the retailers own. You will find some of my retail projects in this repository:


## **1. online-shoppers-intention.csv** __<p>See Notebook <a href="https://github.com/ninaroal/DS-retail/blob/main/online-shoppers-intention.ipynb?plain=1" title="Title"> HERE</a> </p>__

**Business Case - Online Shoppers Purchasing intention:** A company wants to classify customers based on the probability of generating income when shopping on the web.

Several techniques where used for the EDA and modeling:
1.	Handling of missing values
2.	Treatment of categorical variables (one-hot encoder)
3.	Treatment of numerical variables (standardization and normality distribution check)
4.	Visualization of the features and target (boxplots, bar charts, histograms, heatmaps)
5.	Treatment of outliers
6.	Correlations and multicollinearity between features
7.	Building models with hyperparameters (Logistic Regression, SCV and Random Forest Classification)
8.	Comparing models and analyzing metrics (e.g. accuracy, precision and recall). 
The original dataset was extracted from the following website: https://archive.ics.uci.edu/ml/machine-learning-databases/00468/online_shoppers_intention.csv


## **2. creditcard-transactions-anomaly-detector.ipynb** __<p>See Notebook <a href="https://github.com/ninaroal/DS-retail/blob/main/creditcard-transactions-anomaly-detector.ipynb?plain=1" title="Title"> HERE</a> </p>__

**Business Case - Payments Fraud Detection:** Since in real-world case scenarios, it is not feasible to analyze a huge amount of transactions, unsupervised models are very usefull for a first screening to filter out the total number of transactions that are anomalous. This is known as **Anomaly detectors** and they will estimate which transactions are abnormal and which are not, after the anonmalous transactions are audited, the real labels (Y) can be obtained and at some point, the instituion would have reached sufficient labeled data (X, Y) that it can be use to perform a supervised learning classifier.

**Approach of this project:**
In this dataset, we have the characteristics of each transaction (X) and the label indicating whether they are fraud or not (Y). We could directly perform a supervised learning classifier, but the goal for this business case is to have an approximation of how useful an anomaly detection model can be in previous steps.

1. I'm going to assume first that there is no label (Y) and make an anomaly detection model with only the features (X)
2. I will find which transactions I get as abnormal and then compare to the actual labels (Y). In this way we can see how an anomaly detector could serve in that first filtering.
3. I will represent the accumulated profit that we obtain between having a model and not having it.
