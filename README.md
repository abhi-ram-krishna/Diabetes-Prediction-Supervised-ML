# Diabetes-Prediction-Supervised-ML
This project explores the effectiveness of machine learning techniques in predicting diabetes based on various clinical, genetic, and lifestyle factors. Please note that the datasets, including the training and test datasets, as well as the exported models, have been uploaded to [Google Drive](https://drive.google.com/drive/folders/1phQRFL1RVygEyWSxM9l736VS-x0i2slb?usp=sharing) due to the file size limit enforced by Git.
<br>                          
## Goal of the Project
The primary goal of this project is to develop a model that predicts the likelihood of diabetes or pre-diabetes based on input parameters such as gender, age, symptoms, and lifestyle factors. Additionally, the project aims to analyze the risk factors that are most predictive of diabetes risk while testing the usability of BRFSS in providing accurate predictions.
<br>                           
## Data Story
**Total Instances** : 253680             
**Number of Attributes** : 22 (*21 features, 1 Target*)           
**Target Variable** : Diabetes_binary (Categorical, Binary: 0 = no diabetes 1 = prediabetes or diabetes)                     
| Variable Name           | Role    | Type    | Demographic        | Description                                                                                                                                   |
|-------------------------|---------|---------|--------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|     
| target         | Target  | Binary  |                    | **0** = no diabetes, **1** = prediabetes or diabetes                                                                                                |
| HighBP                  | Feature | Binary  |                    | **0** = no high BP, **1** = high BP                                                                                                                 |
| HighChol                | Feature | Binary  |                    | **0** = no high cholesterol, **1** = high cholesterol                                                                                               |
| CholCheck               | Feature | Binary  |                    | **0** = no cholesterol check in 5 years, **1** = yes cholesterol check in 5 years                                                                   |
| BMI                     | Feature | Integer |                    | Body Mass Index                                                                                                                              |
| Smoker                  | Feature | Binary  |                    | Have you smoked at least 100 cigarettes in your entire life? [Note: 5 packs = 100 cigarettes] **0** = no, **1** = yes                               |
| Stroke                  | Feature | Binary  |                    | (Ever told) you had a stroke. **0** = no, **1** = yes                                                                                               |
| HeartDiseaseorAttack    | Feature | Binary  |                    | Coronary heart disease (CHD) or myocardial infarction (MI) **0** = no, **1** = yes                                                                  |
| PhysActivity            | Feature | Binary  |                    | Physical activity in past 30 days - not including job. **0** = no, **1** = yes                                                                      |
| Fruits                  | Feature | Binary  |                    | Consume fruit 1 or more times per day. **0** = no, **1** = yes                                                                                      |
| Veggies                 | Feature | Binary  |                    | Consume vegetables 1 or more times per day. **0** = no, **1** = yes                                                                                 |
| HvyAlcoholConsump       | Feature | Binary  |                    | Heavy drinkers (adult men having more than 14 drinks per week and adult women having more than 7 drinks per week). **0** = no, **1** = yes         |
| AnyHealthcare           | Feature | Binary  |                    | Have any kind of health care coverage, including health insurance, prepaid plans such as HMO, etc. **0** = no, **1** = yes                         |
| NoDocbcCost             | Feature | Binary  |                    | Was there a time in the past 12 months when you needed to see a doctor but could not because of cost? **0** = no, **1** = yes                       |
| GenHlth                 | Feature | Integer |                    | Would you say that in general your health is: (scale 1-5) **1** = excellent, **2** = very good, **3** = good, **4** = fair, **5** = poor                        |
| MentHlth                | Feature | Integer |                    | Now thinking about your mental health, which includes stress, depression, and problems with emotions, for how many days during the past 30 days was your mental health not good? (scale 1-30 days) |
| PhysHlth                | Feature | Integer |                    | Now thinking about your physical health, which includes physical illness and injury, for how many days during the past 30 days was your physical health not good? (scale 1-30 days) |
| DiffWalk                | Feature | Binary  |                    | Do you have serious difficulty walking or climbing stairs? **0** = no, **1** = yes                                                                  |
| Sex                     | Feature | Binary  | Sex                | **0** = female, **1** = male                                                                                                                        |
| Age                     | Feature | Integer | Age                | 13-level age category **1** = 18-24, **2** = 25-29, **3** = 30-34, **4** = 35-39, **5** = 40-44, **6** = 45-49,  **7** = 50-54,  **8**= 55-59, **9** = 60-64, **10** = 65-69,  **11** = 70-74, **12** = 75-79, **13** = 80+                                                         |
| Education               | Feature | Integer | Education Level    | Education level (scale 1-6) **1** = Never attended school or only kindergarten, **2** = Grades 1-8 (Elementary), **3** = Grades 9-11 (Some high school), **4** = Grade 12 or GED (High school graduate), **5** = College 1-3 years (Some college or technical school), **6** = College 4+ years (College graduate) |
| Income                  | Feature | Integer | Income             | Household Income Category (scale 1-8):  **1** = Less than 10,000, **2** = 10,000 to 14,999, **3** = 15,000 to 19,999 **4** = 20,000 to 24,999, **5**  = 25,000 to 34,999,  **6** = 35,000 to 49,999,  **7** = 50,000 to 74,999,  **8** = 75,000 or more |
                                  
<br><br>
## Requirements
List of required libraries and packagges can be found in [installed packages.txt](https://github.com/abhi-ram-krishna/Diabetes-Prediction-Supervised-ML/blob/main/installed_packages.txt).
<br>
## Project Work flow      
This project involves the following steps:<br>
1. **EDA and Preprocessing Data**: the dataset preprocessed by eliminating possible null entries and duplicates. Data exploration is done both by using python libraries and visualizations. Encoded features are exported for upcoming phases.
2. **Model training**: machine learning models are trained on the preprocessed dataset. The models used for this project are `Logistic Regression`, `Decision Tree Classifier` and `Random Forest Classifier`.
3. **Model evaluation**: The trained models are evaluated on the test data to measure its accuracy in detecting diabetes.        
<br><br>
## Conclusion     
### The **Random Forest Classifier** achieved accuracy around **94 %** without tuning or dimensionality reduction.
