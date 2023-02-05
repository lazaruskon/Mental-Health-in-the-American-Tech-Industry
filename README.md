# Mental Health in the American Tech Industry

# Ironhack Mid-term Project: Banking Marketing

![logo_ironhack_blue 7](https://coursereport-s3-production.global.ssl.fastly.net/uploads/school/logo/84/original/logo-ironhack-blue.png)

<h1>Project Maintenance & Contact Details</h1>

The sole contributor to this project is [Lazarus Kon](https://github.com/lazaruskon). This project has been part of my final analysis project of the Ironhack bootcamp I followed (Cohort: Data Analysis Part-time July 2022 - January 2023). For any questions, you can reach out me on my [email address](lazaruskon@gmail.com).

<h1>What are you going to see on this project?</h1>

This repo includes four Jupyter Notebooks used for variious stages of my analysis. We also include links to a presentation on [Canva](https://www.canva.com/design/DAFYMS0ptmk/kQieJH3YlV_TsNN8nv5Fiw/view?utm_content=DAFYMS0ptmk&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink) and a Tableau Dashboard. For this interactive Dashboard a [Desktop version](url here) and a [Laptop version](url here).

<h1>Data Source</h1>

You can find the original datasets [here](https://www.kaggle.com/osmihelp/datasets).

Original Source: [OSMI - Research](https://osmihelp.org/research.html).

Open Sourcing Mental Health (OSMI) is a non-profit, 501(c)(3) corporation dedicated to raising awareness, educating, and providing resources to support mental wellness in the tech and open source communities. EIN: 81-3587896

<h1>Description of Dataset</h1>

The data is . 

The classification goal is to predict if the client will subscribe to a term deposit or not (variable y).

<h1>Feature Description</h1>

Bank client data:
- Age (numeric)
- Job : type of job (categorical: 'admin.', 'blue-collar', 'entrepreneur', 'housemaid', 'management', 'retired', 'self-employed', 'services', 'student', 'technician', 'unemployed', 'unknown')
- Marital : marital status (categorical: 'divorced', 'married', 'single', 'unknown' ; note: 'divorced' means divorced or widowed)
- Education (categorical: 'basic.4y', 'basic.6y', 'basic.9y', 'high.school', 'illiterate', 'professional.course', 'university.degree', 'unknown')
- Default: has credit in default? (categorical: 'no', 'yes', 'unknown')
- Housing: has a mortgage? (categorical: 'no', 'yes', 'unknown')
- Loan: has personal loan? (categorical: 'no', 'yes', 'unknown')

Related with the last contact of the current campaign:
- Contact: contact communication type (categorical: 'cellular','telephone')
- Month: last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')
- Day_of_week: last contact day of the week (categorical: 'mon','tue','wed','thu','fri')
- Duration: last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.

Other attributes:
- Campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
- Pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)
- Previous: number of contacts performed before this campaign and for this client (numeric)
- Poutcome: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')

Social and economic context attributes
- Emp.var.rate: employment variation rate - quarterly indicator (numeric)
- Cons.price.idx: consumer price index - monthly indicator (numeric)
- Cons.conf.idx: consumer confidence index - monthly indicator (numeric)
- Euribor3m: euribor 3 month rate - daily indicator (numeric)
- Nr.employed: number of employees - quarterly indicator (numeric)

Output variable (desired target):
- y - has the client subscribed to a term deposit? (binary: 'yes', 'no')

<h1>About our project</h1>

Project goals included:
 1. finding ways of increasing the positive responses of clients in regards to a term deposit subscription.
 2. creating client profiles of people who, according to our data, are more likely to reply yes when a term deposit subscription is proposed to them.

This project is valuable since it allows us to analyze client behavior and attributes in the midst of the financial crisis of the previous decade that hit South European countries particularly hard.

<h1>Tools & Methods of Analysis</h1>

We used a variety of instruments, libraries and models to achieve the aforementioned goals. Among others we used: 
- Pandas
- Numpy
- Matplotlib
- Seaborn
- scikit-learn
- math
- Supervised learning models for classification:
  - Random Forest
  - Logistic Regression
  - KNeighbors
  - MLP
  - Support Vector Machine
  - XGboost

<h1>Provisional Results & Conclusions</h1>

Comparing all the above models, we concluded that despite our efforts the highest recall score for 1 (Yes) is 0.62, with the overall values ranging from 0.43 to 0.62. Correspondingly, the highest recall score for 0 (No) is 0.94, with the overall values ranging from 0.88 to 0.94. Moreover, we observed high accuracy scores across the board, but quite low F1 scores (for Yes).

Overall, the best performing combination of dataframes and scalers for 1 (Yes) is the standard scaler on the dataframe based on the feature importance, including all outliers. The same for 0 (No) is the polynomial features for the data frame that includes all features but no outliers.

Finally, applying oversampling or undersampling techniques has not significantly improved our models' scores. A trend we observed is that SMOTE tends to slightly increase recall but dramatically decrease precision. The exact opposite is true when we apply TomeKLinks with reducing recall to increase precision.

Based on all these observations we decided to use the Logistic Regression (Important Original Data / Scaler 1) as our reporting result. We're building confidence intervals for this model's recall scores next. Confidence Intervals: With 95% probability the true recall of 0 (No) is in between 0.882 and 0.897. For class 1 (Yes) the true recall is between 0.588 and 0.651 with a 95% probability. 

For more details and a better understanding of these results and conclusions we invite you to check out our Notebook.

<h2>Table of Content of Jupyter Notebook</h2>

- 1. <b>Attribute Information</b>
  - 1.1. Importing Dependencies & Loading the Data
- 2. <b>Data Cleaning</b>
  - 2.1. Nan Values
  - 2.2. Feature Cleaning
- 3. <b>Explanatory Data Analysis</b>
  - 3.1. Checking the Normality of the Target Variable
  - 3.2. Continuous Variables
  - 3.3 Categorical Variables
    - 3.3.1. Visualizing our Target Variable
  - 3.4. Collinearity
    - 3.4.1. Bivariate Analysis
    - 3.4.2. Correlation Matrix
  - 3.5. Checking for Outliers
    - 3.5.1. Removing Outliers
  - 3.6. Feature Selection
- 4. <b>Preprocessing</b>
  - 4.1. Encoding Categorical Features
    - 4.1.1. Encoding Target Variable
  - 4.2. Train / Test Split
  - 4.3 Random Forests
    - 4.3.1. Random Forest for Feature Importance (Original Data)
    - 4.3.2. Random Forest for Feature Importance (Clean Data)
  - 4.4. Train / Test Split with Important Features
- 5. <b>Creating Predictive Models</b>
  - 5.1 Baseline Logistic Regression
  - 5.2 KNeighbors Classifier Application & Evaluation
  - 5.3. MLP Classifier Application & Evaluation
  - 5.4 Addressing Imbalance with SMOTE
  - 5.5. Addressing Imbalance with TomeKLinks
- 6. <b>Additional Models</b>
  - 6.1. Support Vector Machine
  - 6.2. XGboost
- 7. <b>Model Selection</b>
  - 7.1. Confidence Intervals

