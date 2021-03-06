# Titanic_Survival_Prediction
   
### Background problem / Goal:
The challenge of this project was to use a machine learning model to predict passenger survival on the Titanic, i.e. given the data of a new passenger, we want to predict whether they will survive the disaster.
![Titanic](https://github.com/pbamoo/Data-Science-Bootcamp-Projects/blob/main/Week2_Classifiction/Images/stoewer_titanic.jpg)
                   
      Sinking of the Titanic/Untergang der Titanic, by Willy Stöwer, 1912, public domain

### Tools/Libraries Used: 
Python, Pandas, Matplotlib, Seaborn, Scikit-learn

### Workflow:
1. Data Acquisition: 
The [dataset](https://github.com/pbamoo/Data-Science-Bootcamp-Projects/tree/main/Week2_Classifiction/Data) used in this project can be found in the [data folder](https://github.com/pbamoo/Titanic_Survival_Prediction/tree/main/Data). 
   * Features/Variables in our dataset:
      - pclass: A proxy for socio-economic status, 1st (upper), 2nd(middle) and 3rd(lower) class. 
      - sibsp: refers to family relations onboard defined as Sibling + Spouse.
      - parch: refers to parent, child family relations.
      - Age, Sex, Name, Ticket, Fare, Cabin, Embarked, and target variable, Survived.

2. Preprocessing:
In order to prepare the data for machine learning, we will do some preprocessing including handling the missing data, feature transformation and selection, etc. See this [here](https://github.com/pbamoo/Titanic_Survival_Prediction/blob/main/Code/Feature%20Engineering.ipynb).
![alttext](https://github.com/pbamoo/Data-Science-Bootcamp-Projects/blob/main/Week2_Classifiction/Images/Total%20Survival%20Rate%20on%20the%20Titanic.png) 
*Fig. 1: Total Survival Rate on the Titanic*

3. Exploratory Data Analysis(EDA):
A glimpse of data and its context, as well as insights captured using descriptive statistics and visualization techniques can be found [here.](https://github.com/pbamoo/Titanic_Survival_Prediction/blob/main/Code/EDA.ipynb).
![Survival based on various features](https://github.com/pbamoo/Data-Science-Bootcamp-Projects/blob/main/Week2_Classifiction/Images/Survival%20based%20on%20various%20features.png)
*Fig. 2: Survival based on various features*

![Survival based on Age and Gender](https://github.com/pbamoo/Data-Science-Bootcamp-Projects/blob/main/Week2_Classifiction/Images/Survival%20based%20on%20Sex%20%26%20Age.png)
*Fig. 3: Survival based on Age and Gender*                                      

4. Modeling & Evaluation:
Several [classification models](https://github.com/pbamoo/Titanic_Survival_Prediction/blob/main/Code/Modeling.ipynb) were trained and their results compared to ascertain the best performing model and fine tune that model. 
![Confusion Matrix for the Random Forest Model](https://github.com/pbamoo/Data-Science-Bootcamp-Projects/blob/main/Week2_Classifiction/Images/Confusion%20Matrix%20Random%20Forest.png)
*Fig. 4: Confusion Matrix for the Random Forest Model*
         
5. Summary & Outlook:
We started with data exploration, cleaning, feature modification and creation and made predictions using 8 models from which we proceeded with the random forest classifier as the best based on the accuracy. We further proceeded to tune the hyperparameters of our chosen model after which we looked at some further methods of evaluating the model's performance. The results looked promising but of course there is still room for improvement, like doing a more extensive hyperparameter optimization on several models, identifying and removing less important features which create unnecessary noise that interferes with our algorithm.
