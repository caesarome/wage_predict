# wage_predict

## Introduction：

A U.S. employer can hire a foreign worker to work permanently in the U.S. by applying to Department of Labor's permanent larbor certification program(PERM) and providing various information on the employer, the job offered and the employee. In this project, I performed data cleaning and handled missing value firstly, then built a forecasting model to predict the wage of the employee whose application would be approved by PERM. Linear Regression and Random Forest model was used for the analysis and the Random Forest had a better performance on the dataset. 

Data Dictionary in the project:

• case_number: ID of each case

• case_received_date: when the case was received 

• decision_date: when a decision on the case was made

• case_status: the decision on the case

• employer_name: the employer applying for the case 

• employer_num_employees: the number of employees in the employer 

• employer_yr_established: the year the employer was established

• job_education: the educatuin level required for the job

• job_experience_num_month: the expeirence required for the job offered, in months

• job_state: the location of the job

• job_foreign_lang_req: if a foreign language was required for the job

• job_level: the level of the job offered 

• employee_citizenship: the citizenship of the employee

• wage_offer: the lower-end of the wage offered

• wage_unit: the unit of the wage


## Outline：
1. Exploratory Data Analysis
2. Data Cleaning: Impute missing data and create a new feature 'annual_wage'; remove the outliers in annual_wage observations and log transform them; apply one-hot- encoding to the categorical variables in the original dataset and caculate the average annual wage for each category as a new feature  
3. Input the cleaned data into Linear Regression model and Random Forest model, and evaluated the model results

## Results
1. Linear Regression Model：

  MAE: 11897.598067391895
  MSE: 1840392219.8896956
  RMSE: 42899.792772106666

2. Random Forest：

  MAE: 7233.704545409459
  MSE: 216472254.0654224
  RMSE: 14712.99609411429
