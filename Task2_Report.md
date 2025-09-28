
#Task 2 – Machine Learning Model on Titanic Dataset

##1. Introduction
The goal of this task is to predict **Titanic passenger survival** using machine learning.
We use the **Random Forest Classifier** to build a model based on passenger attributes such as **age, gender, class, and fare.**
The model is evaluated using **accuracy, confusion matrix,** and **feature importance visualization.**

##2. Dataset Description
	The dataset contains **892 rows and 12 columns.**
	Important columns include:
	**Survived** – target variable (0 = Did not survive, 1 = Survived)
	**Pclass** – passenger class
	**Sex** – gender
	**Age** – passenger age
	**SibSp** – number of siblings/spouses aboard
	**Parch** – number of parents/children aboard
	**Fare** – ticket fare
	**Embarked** – port of embarkation

##3. Data Preprocessing
	**Missing values**:
	Age filled with mean
	Embarked filled with mode
	Cabin dropped due to too many missing values
	**Encoding categorical columns:**
	Sex → numeric (male=1, female=0)
	Embarked → numeric (C=0, Q=1, S=2)

##4. **Feature Selection**
	**Features used for modelling**: Pclass, Sex, Age, SibSp, Parch, Fare, Embarked
	**Target variable**: Survived

##5. Model Training
	**Model**: Random Forest Classifier
	**Train/Test Split**: 80% training, 20% testing
	**Training**: Model trained on 712 samples
	**Testing**: Predictions made on 179 samples

##6. Model Evaluation
	**Accuracy:** 81%
	**Confusion Matrix**:
	Predicted: No	Predicted: Yes
Actual: No	91	14
Actual: Yes	20	54
	The model shows good predictive performance on unseen test data.

##7. Feature Importance
	**Most important features**: Sex, Fare, Age
	Other features contributed less but still had some influence.

##8. Visualizations

	**Survival Count** – total survived vs did not survive
	**Survival by Sex** – females survived more than males 
	**Survival by Passenger Class** – higher class survived more 
	**Age Distribution by Survival** – younger passengers had higher survival
	**Fare Distribution by Survival** – higher fare linked to higher survival
	**Feature Importance** – shows which features influenced predictions most
 

##9. Insights
	**Gender and ticket fare** had the strongest impact on survival.
	**Age** also influenced survival, while other features like class and family size had a smaller effect.
	The Random Forest model achieved **81% accuracy**, making it a reliable predictor of Titanic survival.

##10.Conclusion

       The Random Forest model achieved **81% accuracy**, demonstrating good predictive performance on the Titanic dataset.
       Gender (Sex) and ticket fare (Fare) were the most influential features in predicting survival.
       Age also played a significant role, while other factors like passenger class and family size had a smaller impact.
       The model and analysis provide valuable insights into passenger survival patterns and can guide further exploration or decision-making.
       Overall, the task successfully demonstrates data preprocessing, model training, evaluation, and interpretation of results using a real-world dataset.

