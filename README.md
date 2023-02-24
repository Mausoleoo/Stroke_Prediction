# Data Science Stroke Prediction

  - 

## Resources

**Python Version**: 3.9.13

**Packages**: Pandas, NumPy, Matplotlib, Scikit-learn

Dataset: https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

Tutorial ML: https://betterdatascience.com/feature-importance-python/

## Steps

1.- Run Data Cleaning.ipynb to clean data. 
    - Remove NaN values 
    - It will create a CSV file (healthcare-dataset-stroke-data-cleaned.csv)
    
    Columns:
      
      * gender: “Male”, “Female” or “Other”

      * age: age of the patient

      * hypertension: 0 if the patient doesn’t have hypertension, 1 if the patient has hypertension

      * heart_disease: 0 if the patient doesn’t have any heart diseases, 1 if the the patient has a heart disease

      * ever_married: “No” or “Yes”

      * work_type: “children”, “Govt_jov”, “Never_worked”, “Private” or “Self-employed”

      * Residence_type: “Rural” or “Urban”

      * avg_glucose_level: average glucose level in blood

      * BMI: body mass index

      * smoking_status: “formerly smoked”, “never smoked”, “smokes” or “Unknown”*

      * stroke: 1 if the patient had a stroke or 0 if not

2.- Run EDA.ipynb to Data Analysis

    Data distribution as well as counts of values for categorical variables were analyzed and examined. 
    The following are a few highlights from the pivot tables.
    
    ![corr](https://user-images.githubusercontent.com/21091686/221055498-e7950864-6b1e-405b-85b1-684ec9d0e374.png)
    
    
    ![pivot](https://user-images.githubusercontent.com/21091686/221055594-74e2af1f-a5aa-4cdf-95c7-802d497ce782.png)

3.- Run Model Building.ipynb to train and test models

    a) Variables were created into dummy variables and the data were split into training and test.
        (209 rows Stroke, 4653 rows No Stroke)
        
    b) Three models were created (Logistic regression, Support Vector Machine, Random Forest)
        - The three models had bad performance
        
    c) A subsample was obtained because the dataset was unbalanced
        (209 rows Stroke, 221 rows No Stroke)
        
    d) The three models were used again
        - The performance was slightly better 
