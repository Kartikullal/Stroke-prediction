# Heart Stroke Prediction

According to the World Health Organization (WHO) stroke is the 2nd leading cause of death globally, responsible for approximately 11% of total deaths.
This dataset is used to predict whether a patient is likely to get stroke based on the input parameters like gender, age, various diseases, and smoking status. Each row in the data provides relavant information about the patient.

## Implementation of the project

### About the dataset

I have linked the dataset in this repository. You can find the dataset on kaggle as well, [here](https://www.kaggle.com/fedesoriano/stroke-prediction-dataset).

#### Attribute Information

1) id: unique identifier
2) gender: "Male", "Female" or "Other"
3) age: age of the patient
4) hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension
5) heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
6) ever_married: "No" or "Yes"
7) work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
8) Residence_type: "Rural" or "Urban"
9) avg_glucose_level: average glucose level in blood
10) bmi: body mass index
11) smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"*
12) stroke: 1 if the patient had a stroke or 0 if not
*Note: "Unknown" in smoking_status means that the information is unavailable for this patient

### Data Cleaning and preprocessing

1) Checked if there are any duplicate values, and removed all duplicates.
2) Mutated some of the missing values, for example, children below age 5 were given a status of no smoking
3) Removed all NA values

### Data visualization

All the data visualizations can be seen in the folder called EDA in the repository.

### Prediction

We used a classification algorithm, logistic regression, to predict whether a patient will get a stroke or not.
The model performs well with an accuracy of 74.2%. The sensitivity of 84.6% is good since we want to miss as little strokes as possible.
