#  Predicting and Analyzing Factors Influencing Student Academic Performance

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
* Programming Languages: Python.
* Libraries:
  - Data Processing: Pandas, NumPy.
  - Visualisation: Matplotlib, Seaborn, Plotly express
  - Modeling: scikit-learn, statsmodels.
## 5. Key insights discovered
### Social Factors:
- Females generally perform better academically compared to males across various factors like study time and alcohol consumption.
- Excessive or minimal socialization is associated with poorer academic performance due to a lack of balance.
- High alcohol consumption (levels 4-5) consistently correlates with the lowest grades.
### Academic Factors
- Increased study time positively impacts grades, with optimal performance seen at 5-10 hours per week.
- Past class failures strongly negatively affect academic performance.
Students aspiring for higher education tend to score significantly higher.
### Personal Background:
- Students with higher parental education tend to achieve better grades.
- Students whose parents work as teachers have a higher mean grade (13.10) compared to the general population (11.91).
- Urban students perform better academically compared to rural students.

## 6. Hypotheses Based on the Insights
- Students with moderate levels of socialization achieve higher grades than those with extreme levels (too high or too low).
- Alcohol consumption negatively impacts academic performance, with higher levels of consumption leading to poorer grades.
- Students with aspirations for higher education are more motivated and achieve better results.
- Past academic failures are significant predictors of future poor performance.
- Parental education and professional background (e.g., being a teacher) contribute positively to students’ academic success.

## 7. Recommendations Based on Analysis Results
### Gender-Specific Support:

Males: Provide mentorship programs focusing on balancing social activities with academics.
Females: Encourage leadership roles in study groups to share successful strategies.
### Promote a Balanced Lifestyle:
- Encourage moderate socialization through school-led clubs and team activities.
- Provide time management training to help students maintain a balance between study and leisure.
### Address Alcohol Consumption:
- Organize awareness campaigns highlighting the negative impact of alcohol on grades.
- Offer alternatives like hobby clubs or non-alcoholic social events.
### Motivate and Support Struggling Students:
- Implement early intervention programs, including tutoring and mentorship for students with prior failures.
- Offer career counseling to emphasize the benefits of higher education.
### Parental and Facilitator Involvement:
- Conduct workshops for parents to equip them with strategies to support their children’s academic growth.
- Establish school-based digital learning hubs to provide internet access and resources for students in need.
