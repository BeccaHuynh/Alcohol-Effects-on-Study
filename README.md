#  Factors impacting Study performance Analysis

## 1. Purpose: 
To identify and evaluate the factors influencing students' performances and predict final academic grades (G3), while answering these questions:
* How do demographic, academic, and social factors interact to influence performance?
* What are the strongest predictors of students’ final grades (G3)?
* Can we build a predictive model to estimate final grades based on the given features?
## 2. Expected Outcome: 
A model that can predict students’ grades with high accuracy, along with insights into factors influencing study performance.

## 3. Dataset Overview:
### Source: 
* Public dataset from Kaggle (Alcohol Effects On Study: [https://www.kaggle.com/datasets/whenamancodes/alcohol-effects-on-study/data](https://www.kaggle.com/datasets/whenamancodes/alcohol-effects-on-study/data) )
* File’s name: Portuguese.csv
### Description: 
*This dataset includes information on 649 students from ages 15 to 22 from two Portuguese schools. The data attributes include student grades, demographic, social and school-related features.*

### Structure:
* school : student's school (binary: 'GP' - Gabriel Pereira or 'MS' - Mousinho da Silveira).
* sex: student's sex (binary: 'F' - female or 'M' - male)
* age: student's age (numeric: from 15 to 22)
* address: student's home address type (binary: 'U' - urban or 'R' - rural)
* famsize: family size (binary: 'LE3' - less or equal to 3 or 'GT3' - greater than 3)
* Pstatus: parent's cohabitation status (binary: 'T' - living together or 'A' - apart)
* Medu: mother's education (numeric: 0 - none, 1 - primary education (4th grade), 2- 5th to 9th grade, 3- secondary education or 4- higher education)
* Fedu: father's education (numeric: 0 - none, 1 - primary education (4th grade), 2- 5th to 9th grade, 3- secondary education or 4- higher education)
* Mjob: mother's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'at_home' or 'other')
* Fjob: father's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'at_home' or 'other')
* reason: reason to choose this school (nominal: close to 'home', school 'reputation', 'course' preference or 'other')
* guardian: student's guardian (nominal: 'mother', 'father' or 'other')
* traveltime: home to school travel time (numeric: 1 - <15 min., 2 - 15 to 30 min., 3 - 30 min. to 1 hour, or 4 - >1 hour)
* studytime: weekly study time (numeric: 1 - <2 hours, 2 - 2 to 5 hours, 3 - 5 to 10 hours, or 4 - >10 hours)
* failures: number of past class failures (numeric: n if 1<=n<3, else 4)
* schoolsup: extra educational support (binary: yes or no)
* famsup: family educational support (binary: yes or no)
* paid: extra paid classes within the course subject (Math or Portuguese) (binary: yes or no)
* activities: extra-curricular activities (binary: yes or no)
* nursery: attended nursery school (binary: yes or no)
* higher: wants to take higher education (binary: yes or no)
* internet: Internet access at home (binary: yes or no)
* romantic: with a romantic relationship (binary: yes or no)
* famrel: quality of family relationships (numeric: from 1 - very bad to 5 - excellent)
* freetime: free time after school (numeric: from 1 - very low to 5 - very high)
* goout: going out with friends (numeric: from 1 - very low to 5 - very high)
* Dalc: workday alcohol consumption (numeric: from 1 - very low to 5 - very high)
* Walc: weekend alcohol consumption (numeric: from 1 - very low to 5 - very high)
* health: current health status (numeric: from 1 - very bad to 5 - very good)
* absences: number of school absences (numeric: from 0 to 93)
* G1: first period grade (numeric: from 0 to 20)
* G2: second period grade (numeric: from 0 to 20)
* G3: final grade (numeric: from 0 to 20, output target)
## 4. Tools and Technologies
Programming Languages: Python.
Libraries:
Data Processing: Pandas, NumPy.
Visualisation: Matplotlib, Seaborn, Plotly express
Modeling: scikit-learn, statsmodels.
## 5. Initial Analysis Plan:
* Data Cleaning: Handle missing values, correct data types, and remove duplicates.
* EDA: Generate summary statistics, visualize distributions, and explore relationships between variables.
* Analysis: Perform correlation analysis, build and evaluate a linear regression model, and identify key factors contributing to study performance.
* Visualization: Create visualizations such as bar charts, histograms, and heatmaps to support the analysis.
* Data Storytelling: Explaining the key drivers of study performance and recommendations for reducing bad grades.

