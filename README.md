# Homework3: Ye Ouyang
# homework-iii-starter
the starter repository for hw3

There are two main files and one folder for data
1) .travis.yml: To configure the Travis and set the environment for test
2) hw3_starter_notebook.ipynb: The file containing the codes

The steps in the code:
1) Data Cleaning
	- load the data
	- Pre-processing (Convert categorical/non-numeric data to numeric data)
	- Feature selection (Select the related features and excluded features which have less impact on the classification)
	- Extract Testing data and Target (The column of "subscribed")
	- Split data into Training and Testing
2) Model Set1: Using 5 models to test, the Feature Engineering and Selection have been done in the above step
	- NearestCentroid
	- KNeighborsClassifier
	- SVC
	- SGDClassifier
	- LogisticRegression
3) Model Set2: Using 3 models to test, the Feature Engineering and Selection have been done in the above step
	- DecisionTreeClassifier
	- RandomForestClassifier
	- GradientBoostingClassifier
4) Model Ensemble: Uising averaging and “poor man’s stacking” method and models created before
5) Resampling
	
