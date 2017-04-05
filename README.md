# Homework3: Ye Ouyang
# homework-iii-starter


There are two main files and one folder for data
1) .travis.yml: To configure the Travis and set the environment for test
2) hw3_starter_notebook.ipynb: The file containing the codes

The steps in the code:
1) Data Cleaning (All data pre-processing and feature engineering/selection are done in this step)
	- Remove the "Duration" attribute which is not related with the modeling
	- Convert categorical data to numeric data
	- Extract traning and target
	- Split training and testing data
	
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
	- From Modelset1: KNeighborsClassifier and LogisticRegression have good acurracy
	- From Modelset2: Decision Tree and Random Forest have good accuracy
	- Use VotingClassifier to ensemble the best results generated from the above two steps
		- LogisticRegression
		- KNeighborsClassifier
		- Decision Tree
		- Random Forest
	- ROC figure is draw here to show the performance of classification
	
5) Travis to test the accuracy: I claim my algorithm is 89% accurate. The following assert statement that score returned by my model is at least 89%
	def test_accuracy():
		assert(ensemble()>0.89)
		
6) Resampling
	
