# Data Science Job Salaries Analysis and Prediction.
According to the 2020 LinkedIn U.S. Emerging Jobs Report, data science has experienced continued growth on a tremendous scale in recent years. Across nearly every industry, organizations are competing for data science professionals to leverage their data and drive smart business decisions. However, since the supply of data professionals has not yet caught up with the demand, the competition between companies in hiring these professionals is fierce compared to in other tech sectors. As a result, employers are willing to pay top salaries to talented data scientists.

Notwithstanding the profitable honeymoon this field is experiencing, it is important to note that the data science salaries can range considerably across professionals. Employers take into account several factors when deciding how much to pay, including experience, skills, job title, or company size.

# LinkedIn Profile
For any queries regarding about this project contact me.

- Link [Click here](https://www.linkedin.com/in/naloys/)

# Acquisition of data
The Data Science salary data (Salary_Data.csv) that we will use for the analysis is obtained from Kaggle.

- Link [Download here](https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries?resource=download)

# Data set
<img width="1247" alt="dataset" src="https://github.com/Bozzer250/Data-Science-Job-Salaries-Analysis-and-Predict/assets/122544599/90a420f8-bc40-4555-86e2-ea866ff72ca0">

## Observation:

• The dataset consists of 12 columns and 607 rows.

- Unnamed: 0
- work_year
- experience_level
- employment_type
- job_title
- salary
- salary_currency
- salaryinusd
- employee_residence
- remote_ratio
- company_location
- company_size

- Column `Unnamed`: 0 needs to be removed, as it is unecessary columns.

- The names of each column are lowercase.

- The values of the `experience_level`, `employment_type`, `remote_ratio`, and `company_size` columns need to be redefined.

- `work_year`, `salary`, `salary_in_usd`, and `remote_ratio` columns are numeric.

# Data Cleansing
- Removed unwanted columns: 'Unnamed: 0'.

- Dataframe has no missing values.

- Drop 42 duplicate rows found.

- Renaming the column value

  - experience_level : EN = Entry-level, MI = Mid-level, SE = Senior-level, EX = Expert-level
  - employment_type : PT = Part-time, CT = Contract, FT = Full-time, FL = Freelance
  - remote_ratio.replace : 0 = Onsite, 50 = Hybrid, 100 = Remote
  - company_size.replace : S = Small, M = Medium, L = Large
    
- After renaming the column value, the dtype of the remote_ratio column changes to object.

## Exploratory Data Analysis (EDA)

### Creating boxplot to see outliers in data.
![output](https://github.com/Bozzer250/Data-Science-Job-Salaries-Analysis-and-Predict/assets/122544599/22ffec53-e44b-41a2-9d5e-13c3e7c3f114)

### Obervations:

- There is no outlier in work_year column.
- There are some outliers in the salary and salary_in_usd columns.
## Feature Correlation
![image](https://github.com/Bozzer250/Data-Science-Job-Salaries-Analysis-and-Predict/assets/122544599/6aae6927-810a-4c1e-a08a-23dc3ef9a97a)

### Observation :

- experience_level and salary_in_usd have a high correlation.
## Analysis 1: What is job with the highest salary in Data Science?

![image](https://github.com/Bozzer250/Data-Science-Job-Salaries-Analysis-and-Predict/assets/122544599/d2ef6a54-b855-4661-b6ab-485a27828745)

### Observations :

- The chart shows that the highest salary by Data Analytics Lead is > 400,000 USD and the lowest by 3D Computer Vision Researcher is < 3,000 USD.
- The average salary of workers in the Data Science field is 100,000 USD.
  
## Analysis 2: What are the top 10 data science jobs in 2022?
![image](https://github.com/Bozzer250/Data-Science-Job-Salaries-Analysis-and-Predict/assets/122544599/0910ccba-5451-449b-add2-ee389c4a2f70)

### Observation:

- In 2022, the top 10 popular data science jobs are shown on the chart and the most popular is Data Engineer.
- Data Scientist, Data Engineer, Data Analyst are the top 3 most popular jobs based on the data.
  
## Analysis 3: How does the remote-ratio vary from year 2020 -2022?

![image](https://github.com/Bozzer250/Data-Science-Job-Salaries-Analysis-and-Predict/assets/122544599/0933f37e-357a-4b57-a32c-691f79917129)

### Observations:

- From 2020 to 2022 there will be an increase in the rate of remote work by Data Science workers.
- The chart shows the existence of a new culture that is most favored by Data Science workers, namely remote / work from home.
  
## Analysis 4: Does salary of employees (salary_in_usd) depends on the exprience level?
![image](https://github.com/Bozzer250/Data-Science-Job-Salaries-Analysis-and-Predict/assets/122544599/d666e747-1021-412f-9948-144537f3b795)

### Observation :

- Experience level highly effects the amount of salary.
### Analysis 5: How is the distribution of Data Science worker locations?
![image](https://github.com/Bozzer250/Data-Science-Job-Salaries-Analysis-and-Predict/assets/122544599/61489e27-a5bd-498a-9fa8-bac4e4c2160d)
### Observation:

- Workers mostly are from american (US) companies.

🙂





