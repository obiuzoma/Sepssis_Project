# Sepsis_Prediction_fastApi

# Sepsis Prediction

Sepsis is a life-threatening medical condition characterized by a systemic inflammatory response to infection, leading to organ dysfunction and failure.

The project aims to predict sepsis by utilizing a predictive model that takes into account various input features, including Plasma glucose level, Blood Work Result-1, Blood Pressure, Blood Work Result-2, Blood Work Result-3, Body mass index, Blood Work Result-4, Patient's age, and the presence of insurance. The goal is to develop a comprehensive prediction system for identifying sepsis risk in patients based on these key input variables.

## 1. Business Understanding

The primary objective of this project is to develop a predictive model for sepsis detection in patients within the Intensive Care Unit (ICU). Sepsis is a life-threatening condition, and early detection is crucial for timely intervention and improved patient outcomes. The business goal is to enhance patient care by providing healthcare professionals with a tool that can assess the likelihood of sepsis development based on key clinical indicators.

### 1.1. Questions

- Is there a statistically significant difference in plasma glucose levels between sepsis and non-sepsis cases?
- Are there specific patterns or thresholds in Blood Work Results associated with a higher likelihood of sepsis?
- Are there identifiable trends or correlations between blood pressure levels and the likelihood of developing sepsis?
- Is there a correlation between BMI and the risk of sepsis?
- Is there a specific age group more susceptible to sepsis?
- Is there any correlation between insurance status and the likelihood of developing sepsis?
- Are certain combinations of variables more indicative of sepsis risk?
- What are the key factors contributing to the model's performance or limitations?
- How prevalent is Sepsis among ICU patients?

### 1.2. Objectives

- Investigate the distribution of plasma glucose levels among patients with and without sepsis.
- Compare the distributions of Blood Work Results for patients with and without sepsis.
- Examine the relationship between blood pressure values and the occurrence of sepsis.
- Analyze the distribution of Body Mass Index among individuals with and without sepsis.
- Explore the age distribution of patients with sepsis compared to those without.
- Determine the percentage of patients with valid insurance among those with and without sepsis.
- Assess how well combined factors predict sepsis occurrence.
- Evaluate the accuracy of the predictive model in identifying sepsis based on selected features.
- To see the prevalence of Sepsis among ICU patients.

### 1.3. Hypotheses

#### Plasma Glucose Levels and Sepsis:

- H0: There is no significant difference in the distribution of plasma glucose levels between patients with sepsis and those without sepsis.
- H1: There is a significant difference in the distribution of plasma glucose levels between patients with sepsis and those without sepsis.

#### Blood Work Results and Sepsis:

- H0: The distributions of Blood Work Results are similar for patients with and without sepsis.
- H1: There is a significant difference in the distributions of Blood Work Results between patients with sepsis and those without sepsis.

#### Blood Pressure Values and Sepsis:

- H0: There is no association between blood pressure values and the occurrence of sepsis.
- H1: There is a significant relationship between blood pressure values and the occurrence of sepsis.

#### Body Mass Index (BMI) and Sepsis:

- H0: The distribution of Body Mass Index is similar among individuals with and without sepsis.
- H1: There is a significant difference in the distribution of Body Mass Index between individuals with sepsis and those without sepsis.

#### Age Distribution and Sepsis:

- H0: The age distribution is the same for patients with sepsis and those without sepsis.
- H1: There is a significant difference in the age distribution between patients with sepsis and those without sepsis.

#### Insurance Status and Sepsis:

- H0: There is no difference in the percentage of patients with valid insurance between those with and without sepsis.
- H1: There is a significant difference in the percentage of patients with valid insurance between those with sepsis and those without sepsis.

#### Predictive Model and Sepsis Occurrence:

- H0: Combined factors do not predict the occurrence of sepsis.
- H1: Combined factors significantly predict the occurrence of sepsis.

#### Accuracy of Predictive Model:

- H0: The predictive model's accuracy in identifying sepsis based on selected features is not significantly different from random chance.
- H1: The predictive model's accuracy in identifying sepsis based on selected features is significantly better than random chance.

### 1.4. Features and Target

#### 1.4.1. Features

- **PRG (Plasma glucose level):** Level of glucose in the patient's plasma.
- **PL (Blood Work Result-1):** Results of a specific blood test.
- **PR (Blood Pressure):** Patient's blood pressure.
- **SK (Blood Work Result-2):** Another blood test result.
- **TS (Blood Work Result-3):** Another blood test result.
- **M11 (Body mass index):** Patient's body mass index (BMI).
- **BD2 (Blood Work Result-4):** Another blood test result.
- **Age:** Patient's age in years.
- **Insurance:** Binary variable indicating whether a patient holds a valid insurance card.

#### 1.4.2. Target

The target variable, labeled "Sepsis," indicates whether a patient in the ICU will develop sepsis or not. Predicting sepsis development is crucial for timely intervention and improving patient outcomes in the ICU.


### Data Fields

| Column   Name                | Attribute/Target | Description                                                                                                                                                                                                  |
|------------------------------|------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ID                           | N/A              | Unique number to represent patient ID                                                                                                                                                                        |
| PRG           | Attribute1       |  Plasma glucose|
| PL               | Attribute 2     |   Blood Work Result-1 (mu U/ml)                                                                                                                                                |
| PR              | Attribute 3      | Blood Pressure (mm Hg)|
| SK              | Attribute 4      | Blood Work Result-2 (mm)|
| TS             | Attribute 5      |     Blood Work Result-3 (mu U/ml)|                                                                                  
| M11     | Attribute 6    |  Body mass index (weight in kg/(height in m)^2|
| BD2             | Attribute 7     |   Blood Work Result-4 (mu U/ml)|
| Age              | Attribute 8      |    patients age  (years)|
| Insurance | N/A     | If a patient holds a valid insurance card|
| Sepssis                 | Target           | Positive: if a patient in ICU will develop a sepsis , and Negative: otherwise |

### Missing Attribute Values: Yes