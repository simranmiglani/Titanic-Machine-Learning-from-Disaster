# Titanic-Machine-Learning-from-Disaster
Analysed the dataset of the survivors of Titanic shipwreck using pandas, and visualise the data using matplotlib and seaborn.
The dataset was fetched from githubusercontent.com. Here's a brief description of each column in the data.

PassengerID: A column added by Kaggle to identify each row and make submissions easier
Survived: Whether the passenger survived or not and the value we are predicting (0=No, 1=Yes)
Pclass: The class of the ticket the passenger purchased (1=1st, 2=2nd, 3=3rd)
Sex: The passenger's sex
Age: The passenger's age in years
SibSp: The number of siblings or spouses the passenger had aboard the Titanic
Parch: The number of parents or children the passenger had aboard the Titanic
Ticket: The passenger's ticket number
Fare: The fare the passenger paid
Cabin: The passenger's cabin number
Embarked: The port where the passenger embarked (C=Cherbourg, Q=Queenstown, S=Southampton)

The dataset had some missing values in the columns: Age, Cabin and Embarked. The missing values were imputed using SimpleImputer.
Next, pivot table was used to calculate the survival rate for different gender and Pclass combination. Visualized the distribution of Column Age for both survived and non-survived population.
Then, uing sns.barplot, the survival rate for column SibSp and Parch is visualised.
Moving on, the correlations between the feature and the target variable Survived were analysed and visualised using heatmap.
Using sns.FacetGrid, we analysed the correlations between embarkements and the survival rate based on gender, and found out that womean had higher chances of survival at Port Q and S.
To predict the probability of survival for all the passengers, I built a Logistic Regression model.
