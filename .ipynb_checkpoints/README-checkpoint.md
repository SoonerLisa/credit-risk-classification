# credit-risk-classification
Module 20 Challenge

Repository URL: https://github.com/SoonerLisa/credit-risk-classification.git

In this challenge our data source is comprised of equal-leveled lending service companies' historical records of loan activity. If successful the model will assess and accurately identify borrowers' class measured by risk. In this case "Healthy" or "High-Risk."

Spoiler alert, the model did a fine job predicting the class of the borrowers. Let me explain how.

- Accuracy Score - In order to ensure accuracy many factors were considered. Those of loan size, interest rate, borrower income and debt to income, number of accounts by owner, derogatory marks (strikes against their credit report) and total debt.
- Precision Score - To keep precision and prevent trailing data, the first step accounted for their loan status. A score of zero is Healthy (75,036), while a score of one is High-Risk (2,500), for total of 77,536 customers with results in every factor. A complete data set for this challenge were split and weighted unequally with 80% of the data used for training the model, while 20% used for testing it. This split-ration is typical with Logistic Regression models. 
- Recall Score - Was the model able to predict both classes? That is correct. In this case the Recall Score is high. The number of correctly predicted positive observations measured up to actual positive observations. A low Recall Score suggests many missed positive cases.
      Recall Formula
          Recall = TP / (TP + FN)
              True Positives - The # of correctly predicted positive observations.
              False Negatives - The # of actual positive observations that were incorrectly predicted
                  as negative.
- The actual splitting of a database between training and testing is known as the train test split function. The X represents training. The y represents testing. These defined variables were used in a Confusion Matrix which gives us a nice visualization of the Actual and Predicted Positives, Actual and Predited Negatives as shown in the code.
 
- It was satisfying to have a model work so well. It will continue to be trained and tested on similar databases such as this. Most likely to be used for databases in likeness within the banking industry.

Analysis Modules/Tools used: numpy, pandas, python, pathlib, sklearn.metrics with confusion_matrix and classification_report, sklearn for the train_test_split, sklear.linear_model for Logistical Regression, seaborn, matplotlib.pyplot, sklearn.neighbors with KNeighborsClassifier

Code works well in a python dev environment. When written a Python 3 (ipykernal) was used for coding within jupyter notebook.
Environment: dev (python 3.13.0)

No outside references were used in this challenge. Only those recommended and supported by BootCampSpot.