# Predicting-Pain-Reliever-Misuse-Abuse
Repository for analyzing and predicting pain reliever misuse and abuse using the National Survey on Drug Use and Health (2015-2017) dataset. This project includes data preprocessing, exploratory analysis, and building machine learning models to identify risk factors and predict misuse/abuse.

# Dataset Overview
Our dataset contains various demographic and behavioral factors, with the goal of predicting pain reliever misuse or abuse. Each row represents an individual's survey response, and each column contains specific information about that individual.

Column Descriptions
YEAR: The year the survey was conducted. (Integer)
AGECAT: Age category of the respondent. (Categorical)
1: 12-17 years
2: 18-25 years
3: 26-34 years
4: 35-49 years
5: 50-64 years
6: 65 years and older
SEX: Gender of the respondent. (Categorical)
0: Female
1: Male
MARRIED: Marital status of the respondent. (Categorical)
0: Not married
1: Married
EDUCAT: Education level of the respondent. (Categorical)
1: Less than high school
2: High school graduate
3: Some college/Associate's degree
4: Bachelor's degree
5: Advanced degree
EMPLOY18: Employment status of the respondent. (Categorical)
0: Not employed
1: Part-time employed
2: Full-time employed
CTYMETRO: Whether the respondent lives in a city/metropolitan area. (Categorical)
0: Non-metro
1: Metro
HEALTH: Self-reported health status of the respondent. (Categorical)
1: Excellent
2: Very good
3: Good
4: Fair
5: Poor
MENTHLTH: Self-reported mental health status of the respondent. (Categorical)
1: Excellent
2: Very good
3: Good
4: Fair
5: Poor
PRLMISEVR: Whether the respondent has ever misused prescription medications. (Binary)
0: No
1: Yes
PRLMISAB: Whether the respondent has abused prescription medications. (Binary)
0: No
1: Yes
PRLANY: Whether the respondent has misused or abused prescription medications. (Binary)
0: No
1: Yes
HEROINEVR: Whether the respondent has ever used heroin. (Binary)
0: No
1: Yes
HEROINUSE: Whether the respondent has used heroin in the past year. (Binary)
0: No
1: Yes
TRQLZRS: Whether the respondent has used tranquilizers in the past year. (Binary)
0: No
1: Yes
SEDATVS: Whether the respondent has used sedatives in the past year. (Binary)
0: No
1: Yes
COCAINE: Whether the respondent has used cocaine in the past year. (Binary)
0: No
1: Yes
AMPHETMN: Whether the respondent has used amphetamines in the past year. (Binary)
0: No
1: Yes
HALUCNG: Whether the respondent has used hallucinogens in the past year. (Binary)
0: No
1: Yes
TRTMENT: Whether the respondent has received treatment for substance use. (Binary)
0: No
1: Yes
MHTRTMT: Whether the respondent has received treatment for mental health issues. (Binary)
0: No
1: Yes

Sample Data Interpretation
YEAR  AGECAT  SEX  MARRIED  EDUCAT  EMPLOY18  CTYMETRO  HEALTH  MENTHLTH  \
0    15       3    1        0       2         2         0       3         4   

PRLMISEVR  ...  PRLANY  HEROINEVR  HEROINUSE  TRQLZRS  SEDATVS  COCAINE  \
0          1  ...      10          1          5        5        0        5   

AMPHETMN  HALUCNG  TRTMENT  MHTRTMT  
0         2        2        6        0  

YEAR: The survey was conducted in the year 2015.
AGECAT: The respondent belongs to the age category 26-34 years.
SEX: The respondent is male.
MARRIED: The respondent is not married.
EDUCAT: The respondent is a high school graduate.
EMPLOY18: The respondent is employed full-time.
CTYMETRO: The respondent does not live in a metropolitan area.
HEALTH: The respondent's self-reported health status is "Good".
MENTHLTH: The respondent's self-reported mental health status is "Fair".
PRLMISEVR: The respondent has misused prescription medications.
PRLMISAB: Not provided in the sample.
PRLANY: The respondent has misused or abused prescription medications.
HEROINEVR: The respondent has used heroin.
HEROINUSE: The respondent has used heroin in the past year.
TRQLZRS: The respondent has used tranquilizers in the past year.
SEDATVS: The respondent has not used sedatives in the past year.
COCAINE: The respondent has used cocaine in the past year.
AMPHETMN: The respondent has used amphetamines in the past year.
HALUCNG: The respondent has used hallucinogens in the past year.
TRTMENT: The respondent has received treatment for substance use.
MHTRTMT: The respondent has not received treatment for mental health issues.
