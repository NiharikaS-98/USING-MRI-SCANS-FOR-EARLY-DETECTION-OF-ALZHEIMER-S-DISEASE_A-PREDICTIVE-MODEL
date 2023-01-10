# USING-MRI-SCANS-FOR-EARLY-DETECTION-OF-ALZHEIMER'S-DISEASE_A-PREDICTIVE-MODEL
This project aims at designing a machine learning-based predictive model that considers the clinical dementia rating (CDR) (0-healthy, 1-dementia, 2-AD) data from MRI scans to predict the prevalence of AD in a patient. 
USING MRI SCANS FOR EARLY DETECTION OF ALZHEIMER'S DISEASE: A PREDICTIVE MODEL

Alzheimer’s disease (AD) is a progressive neurodegenerative condition characterised by acute dementia. It is an adult-onset cognitive disorder that impacts over 850,000 people with dementia in the United Kingdom. At the current state of prevalence and absence of any known consolidated treatment, this number is estimated to rocket up to 1.5 million by 2040 (Alzheimer’s Society, 2019). Patients suffering from AD show marked decrease in their brain volume specifically the temporal and parietal lobe in comparison to a healthy brain. This reflects as impaired speech, reduced cognitive abilities, and severely compromised memory retention and recall.
The rapid disease progression barely spares any time for the patient to undergo treatment. 
The conventional MRI is built to detect structural abnormalities in the brain thereby limiting the scope of early detection of AD. Fortunately, recent studies in the field of artificial intelligence and machine learning show that efficient AI-based imaging systems are growing to be capable in detecting early-stage AD. Thus, early detection of the disease is the key to buy time for therapies and bargain against the perils of AD.
This project aims at designing a machine learning-based predictive model that considers the clinical dementia rating (CDR) (0-healthy, 1-dementia, 2-AD) data from MRI scans to predict the prevalence of AD in a patient. 



To run:

	1. The code consists of a .ipynb file containing the prediction model for this assignment with clear annotations for every section. 

	2. "oasis_cross-sectional.csv" and "oasis_longitudinal.csv" are the two datasets that are being used 
	    and can be imported directly without the path using pandas function since the datasets are within the same folder structure. 

	3. Each section of the code can be executed separately to view the section-wise outputs 

        4. The folder also has a requirements.txt file containing details of each and every 
	   modules that are imported within the code and their respective versions  

	5. Bulk installation of all these modules can be done by using "pip install -r requirements.txt" in the python terminal.

I made use of various machine learning algorithms including Logistic Regression, Decision Tree Classifier, KNeighbours Classifier, XGBClassifier, and Gradient Boosting Classifier to predict the early detection of Dementia and Alzheimer's disease using MRI scans. The said models were trained on 70% of the data present in the above mentioned datasets with the remaining 30% being used for validation and testing.

As per the model scores received from each classifier, I made a comparison between the training and test accuracies. The Gradient Boosting Classifier was seen to have the highest model score. The models and their respective scores are as follows: 

        Model	                     Train Score          Test Score
0	XGBClassifier	             1.000000	          0.783333
1	GradientBoostingClassifier   0.790041	          0.794444
2	LogisticRegression	     0.763723	          0.705556
3	DecisionTreeClassifier	     0.823389	          0.705556
4	KNeighborsClassifier	     0.787589	          0.683333 


Once the Gradient Boosting Classifier was trained and tested on the given datasets, it provided a precision of 82% for healthy patients, 73% for Dementia, and 79% for Alzheimer's patients respectively. True positive counts and the Type 1, Type 2 errors were carefully plotted in an "Actual" vs "Predicted"  confusion matrix that provided us a detailed analysis of successful predictions by the model.
