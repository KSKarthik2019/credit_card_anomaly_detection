# credit_card_anomaly_detection
It uses LogisticRegression, SVM and Naive Bayes algorithms to create statistical model for classification of fraud transactions.

It is my RP capstone machine learning project. It helps to classify the fraud credit card transaction, based on the given features. It uses cross validation, confusion matrix, ROC-AUC curve, Classification Report for performance measure.

Please refer to C3879C_Capstone_Project_Report_18061866.pdf for more info.

Pseudo Code:
1.	 Load Dataset into the system. 
2.	 Class Count function to check if the dataset is balanced or imbalanced
3.	 Scale Non-Anonymised features such as Time and Amount
4.	 Concatenate both Scaled Amount and Time with Actual Dataset/frame. 
5.	 Drop old Amount and Time features 
6.	 Random under-sampling function
6.1.	Split the scaled dataset into Train and Test
6.2.	Reset index of scaled train and test dataset
6.3.	Find no of fraud transactions in the (random) Training dataset
6.4.	Segregate normal and fraud transactions from the training data
6.5.	Randomly selecting the same no of normal transactions as fraud transactions
6.6.	Reset Index of both selected normal and fraud transactions
6.7.	Concatenate both selected normal and fraud transactions. 
6.8.	Shuffle the subsample/final dataframe. 
7.	Remove extreme outliners and create final dataset
8.	Split final dataset into Train and Test
9.	Spot-check a couple of Classification Algorithms (using cross validation) 
10.	Make Predictions on Test data
11.	Tune the (best) model’s hyperparameters. 
12.	End. 
