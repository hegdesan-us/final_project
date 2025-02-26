# Final Capstone Project

 **Change in the project:** 
Final capstone project has been changed since it was first proposed during first meeting with the TA. Initially, I was intended to do Recommendation system. However, one of the module was fully based on Recommendation system and most of the work I was planning to do was covered in the class module itself. 

Inorder to gain more experience in model building, I have opted for weight loss analysis. This project is directly related to the area of work as the current company.  I could use this learning to build better models in the existing Fitness app.

 **URL for the assignment:** 
```
https://github.com/hegdesan-us/final_project.git
```
 **URL for solution Jupyter notebook:** 
```
https://github.com/hegdesan-us/assignment_17/blob/c0b910b7f9078b128a4f284e30b062b9fa5ab0d4/prompt_III.ipynb
```

**Name :** Sanjay Hegde \
**Couse :** UCB AI/ML 

**Directory :** Images \
  Description : Contains the images needed for the prompt questions and the Jupyter notebook 

**Directory : data** \
 Description : Contains the data file needed for the class project\
 Contains file : dailyActivity_merged.csv

### Data Preperation
 **Not much missing values**

 ![MissingDataImage](images/missing.png)


## Exploratory Data Analysis (EDA)

**From the bivariate analysis**
- Clearly there are some zero values for Total Distance and Calories which we will need to clean up (i.e., remove) in data prep
- Concentration of users with total distance between 3 to 15 miles and Calories between 1000 to 4000
- Few outliers over 20 miles but still with Calories between 1000 to 4000. Although a couple over 25 miles with Calories over 4000
- Limited records with Total Distance over 25k miles and Calories over 4000##
- Strong correlation between Total Steps taken and Distance. As the TotalDistance increases, the TotalSteps also increase showing a linear relationship between the two features.
- Interesting observations with folks logging zero active minutes but recording values for Total Distance. Maybe Fitbit not working and bad data. These are  candidates to be removed during data preparation (i.e., remove records where Very Active Minutes is zero)
- We have 33 unique users in the dataset recording their activities over a number of days. Max no of days for some records is 31 days (i.e., one month) Let's explore one user and visualize their activities over that one month period.

**From the heatmap:**
- Strong correlation between Total Distance and Tracker Distance. Very Active Distance also shows a strong correlation with Total Distance and Tracker Distance features.

- However, there is weak correlation across the board between the computed weight loss features and the other features.


**From univariate analysis**
- LoggedActivitiesDistance, VeryActiveDistance, ModeratelyActiveDistance, LightActiveDistance and SedentaryActiveDistance may not be valuable for modelling. We can remove them
- There are some rows with Calories = zero and Total Distance = zero as these records are not useful


<h2> Visualizations</h2>

**Univariate Data Analysis**

 ![Numarical Univariate analysis](images/univariate.png)


**Bivariate Data Analysis**

 ![Bivariate Data analysis](images/bivariate.png)


**Correlation Heatmap**

![Correlationheatmap](images/correlation.png)
 

 
## Major features for the Machine Learning Models SelectKBest feature selection
- Selected Features: To be determined

## Model performance comparision
Now, we aim to compare the performance of the Logistic Regression model to our KNN algorithm, Decision Tree, and SVM models.  Using the default settings for each of the models, fit and score each.  Also, be sure to compare the fit time of each of the models.  Present your findings in a `DataFrame` similar to that below: 


(To be determined)
| __Machine Learning Models__| __Train Time (sec)__| __Train Accuracy__|__Test Accuracy__|__Precision__|__Recall__|__F1 Score__|
| :-:| :-:| :-:|:-:|:-:|:-:|:-:|
|  Baseline   |  0.0 |0.0    |0.0    | 0 | 0 |0 |
|  Log Reg    | 0.0 |0.0    |0.0    | 0 | 0 |0 |
|  KNN   | 0.0 |0.0    |0.0    | 0 | 0 |0 |
|  SVM   |  0.0 |0.0    |0.0    | 0 | 0 |0 |
|  RF   | 0.0 |0.0    |0.0    | 0 | 0 |0 |
|  DTree   |  0.0 |0.0    |0.0    | 0 | 0 |0 |


**Next steps**

- Iterate through models based on selective features for better  model


 

 
