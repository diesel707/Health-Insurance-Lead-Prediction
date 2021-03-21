# Health-Insurance-Lead-Prediction-using-Logistic-Regression

The main aim of the algorithm was to identify whether or not an individual will buy a health insurance based on some attributes given in a dataset. 

For the algorithm, the python libraries used were : 
Pandas 

Numpy 

Scikit-Learn

The dataset had following columns : 

ID,	City_Code,	Region_Code,	Accomodation_Type,	Reco_Insurance_Type,	Upper_Age,	Lower_Age,	Is_Spouse,	Health Indicator,	Holding_Policy_Duration,	Holding_Policy_Type,	Reco_Policy_Cat,	Reco_Policy_Premium and	Response


The dataset had categorical data, ordinal data and numerical data. 

The NaN values were treated. Then, using corr() the correlation between columns were found.

I used column; Accomodation_Type,	Reco_Insurance_Type,	Upper_Age,	Lower_Age and	Reco_Policy_Cat to predict the result.

Remaining columns were dropped.

Then the data was normalized and scaled using RobustScaler().

Afterwards, I used Stratified K-fold with Random Forest Classifier to obtain the results. Also, I used Bagging to obtain a better accuracy.

Mean Validation ROC AUC value of the algorithm was : 0.5858425235444984

For a much larger dataset, we can use Stratified K-fold with logistic regression to obtain better results.
