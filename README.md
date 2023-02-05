# Mental Health in the American Tech Industry

![logo_ironhack_blue 7](https://coursereport-s3-production.global.ssl.fastly.net/uploads/school/logo/84/original/logo-ironhack-blue.png)

<h1>Project Maintenance & Contact Details</h1>

The sole contributor to this project is [Lazarus Kon](https://github.com/lazaruskon). This project has been part of my final analysis project of the Ironhack bootcamp I followed (Cohort: Data Analysis Part-time July 2022 - January 2023). For any questions, you can reach out me on my [email address](lazaruskon@gmail.com).

<h1>What are you going to see on this project?</h1>

This repo includes four Jupyter Notebooks used for variious stages of my analysis. We also include links to a presentation on [Canva](https://www.canva.com/design/DAFYMS0ptmk/kQieJH3YlV_TsNN8nv5Fiw/view?utm_content=DAFYMS0ptmk&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink) and a Tableau Dashboard. For this interactive Dashboard a [Desktop version](url here) and a [Laptop version](url here).

<h1>Data Source</h1>

You can find all datasets use for this project [here](https://www.kaggle.com/osmihelp/datasets).

Original Source: [OSMI - Research](https://osmihelp.org/research.html).

Open Sourcing Mental Health (OSMI) is a non-profit, 501(c)(3) corporation dedicated to raising awareness, educating, and providing resources to support mental wellness in the tech and open source communities. EIN: 81-3587896

<h1>Description of Dataset</h1>

The data is compised of multiple annual surveys filled out by tech employees globally. With over 120 features (see below under Feature Description) the surveys aim to describe the experience of tech employees in regards to mental health issues within their workplace.

<h1>Feature Description & Relabeling</h1>

- '#' - (unique ID),

1. Current Employement

- Are you self-employed? = 'self_employed' (0 = No, 1 = Yes),
- How many employees does your company or organization have? = 'n_employees',
- Is your employer primarily a tech company/organization? = 'tech_company' (0 = No, 1 = Yes),
- Is your primary role within your company related to tech/IT? = 'tech_job' (0 = No, 1 = Yes),
- Does your employer provide mental health benefits\xa0as part of healthcare coverage? = employer_MH_benefits (Yes, I don't know, No, Not Eligible for coverage / NA),
- Do you know the options for mental health care available under your employer-provided health coverage? = knows_coverage (Yes, No),
- Has your employer ever formally discussed mental health (for example, as part of a wellness campaign or other official communication)? = formal_discussion (Yes, No, I don't know),
- Does your employer offer resources to learn more about mental health disorders and options for seeking help? = learning_resources (Yes, No, I don't know),
- Is your anonymity protected if you choose to take advantage of mental health or substance abuse treatment resources provided by your employer? = anonymity_protected (Yes, No, I don't know),
- If a mental health issue prompted you to request a medical leave from work, how easy or difficult would it be to ask for that leave? = ask_MH_leave,
- Would you feel more comfortable talking to your coworkers about your physical health or your mental health? = talk_about_health (Physical health, Same level of comfort for each, Mental health),
- Would you feel comfortable discussing a mental health issue with your direct supervisor(s)? = discuss_MH_supervisor (Yes, No, Maybe),
- Have you ever discussed your mental health with your employer? = ever_discuss_employer (0 = No, 1 = Yes),
- Describe the conversation you had with your employer about your mental health, including their reactions and what actions were taken to address your mental health issue/questions. = describe_discussion_employer (various descriptions),
- Would you feel comfortable discussing a mental health issue with your coworkers? = discuss_MH_coworker (Yes, No, Maybe),
- Have you ever discussed your mental health with coworkers? = ever_discuss_coworker (0 = No, 1 = Yes),
- Describe the conversation with coworkers you had about your mental health including their reactions. = 'describe_discussion_coworker' (various descriptions),
- Have you ever had a coworker discuss their or another coworker's mental health with you? = coworker_discuss_coworker (0 = No, 1 = Yes),
- Describe the conversation your coworker had with you about their mental health (please do not use names). = describe_coworker_discussion_coworker (various descriptions),
- Overall, how much importance does your employer place on physical health? = importance_employer_PH (1 - 10 scale),
- Overall, how much importance does your employer place on mental health? = importance_employer_MH (1 - 10 scale),
- Do you have medical coverage (private insurance or state-provided) that includes treatment of mental health disorders? = MH_medical_coverage (0 = No, 1 = Yes),
- Do you know local or online resources to seek help for a mental health issue? = knows_MH_resources (I know some, Yes, I know several, No, I don't know any),
- If you have been diagnosed or treated for a mental health disorder, do you ever reveal this to clients or business contacts? = reveal_MH_client ('Not applicable to me', 'No, because it would impact me negatively', 'Sometimes, if it comes up', 'No, because it doesn't matter', 'Yes, always'),
- If you have revealed a mental health disorder to a client or business contact, how has this affected you or the relationship? = reveal_MH_effect_client (I'm not sure, Negatively, No change, Positively)
- If you have been diagnosed or treated for a mental health disorder, do you ever reveal this to coworkers or employees? = reveal_MH_coworker ('Not applicable to me', 'No, because it would impact me negatively', 'Sometimes, if it comes up', 'No, because it doesn't matter', 'Yes, always'),
- If you have revealed a mental health disorder to a coworker or employee, how has this impacted you or the relationship? = reveal_MH_effect_coworker (Not applicable to me, I'm not sure, Negatively, No change, Positively),
- Do you believe your productivity is ever affected by a mental health issue? = productivity_affected (Yes, Unsure, Not applicable to me, No),
- If yes, what percentage of your work time (time performing primary or secondary job functions) is affected by a mental health issue? = worktime_affected (1-25%, 26-50%, 51-75%, 76-100%)

2. Previous Employment

- Do you have previous employers? = previous_employers (0 = No, 1 = Yes),
- Was your employer primarily a tech company/organization? = previous_tech_company (0 = No, 1 = Yes),
- Have your previous employers provided mental health benefits? = previous_employer_MH_benefits (Some did, No, none did, I don't know, Yes, they all did),
- Were you aware of the options for mental health care provided by your previous employers? = previous_aware_coverage ('I was aware of some', 'N/A (was not aware)', 'N/A (none offered)', 'Yes, I was aware of all of them', 'No, I only became aware later'),
- Did your previous employers ever formally discuss mental health (as part of a wellness campaign or other official communication)? = previous_formal_discussion ('None did', 'Some did', 'I don't know', 'Yes, they all did'),
- Did your previous employers provide resources to learn more about mental health disorders and how to seek help? = previous_learning_resources ('None did', 'Some did', 'Yes, they all did'),
- Was your anonymity protected if you chose to take advantage of mental health or substance abuse treatment resources with previous employers? = previous_anonymity_protected (I don't know, Yes, always, Sometimes, No),
- Would you have felt more comfortable talking to your previous employer about your physical health or your mental health? = previous_talk_about_health (Physical health, Same level of comfort for each, Mental health),
- Would you have been willing to discuss your mental health with your direct supervisor(s)? = discuss_MH_previous_supervisor ,
- Did you ever discuss your mental health with your previous employer? = ever_discuss_previous_employer (0 = No, 1 = Yes),
- Describe the conversation you had with your previous employer about your mental health, including their reactions and actions taken to address your mental health issue/questions. = describe_discussion_previous_employer (various descriptions),
- Would you have been willing to discuss your mental health with your coworkers at previous employers? = discuss_MH_previous_coworker ('At some of my previous employers', 'No, at none of my previous employers', 'Some of my previous employers', 'Yes, at all of my previous employers'),
- Did you ever discuss your mental health with a previous coworker(s)? = ever_discuss_previous_coworker (0 = No, 1 = Yes),
- Describe the conversation you had with your previous coworkers about your mental health including their reactions. = 'describe_discussion_previous_coworker' (various descriptions),
- Did you ever have a previous coworker discuss their or another coworker's mental health with you? = coworker_previous_discuss_coworker (0 = No, 1 = Yes),
- Describe the conversation your coworker had with you about their mental health (please do not use names) = 'describe_previous_coworker_discussion_coworker' (various descriptions),
- Overall, how much importance did your previous employer place on physical health? = 'importance_previous_employer_PH' (1 - 10 scale),
- Overall, how much importance did your previous employer place on mental health? = 'importance_previous_employer_MH' (1 - 10 scale),

3. Mental Health Diagnosis

- Do you currently have a mental health disorder?' = current_diagnosis (Yes, No, Possibly, Don't Know),
- Have you ever been diagnosed with a mental health disorder?' = ever_diagnosed (Yes, No),

    3.1. Empty disorder columns

- Anxiety Disorder (Generalized, Social, Phobia, etc) = anxiety_disorders_empty (all nans),
- Mood Disorder (Depression, Bipolar Disorder, etc) = mood_disorders_empty (all nans),
- Psychotic Disorder (Schizophrenia, Schizoaffective, etc) = psychotic_disorders_empty (all nans),
- Eating Disorder (Anorexia, Bulimia, etc) = eating_disorders_empty (all nans),
- Attention Deficit Hyperactivity Disorder = ADHD_empty (all nans),
- Personality Disorder (Borderline, Antisocial, Paranoid, etc) = personality_disorders_empty (all_nans),
- Obsessive-Compulsive Disorder = OCD_empty (all_nans),
- Post-Traumatic Stress Disorder = PTSD_empty (all nans),
- Stress Response Syndromes = stress_response_empty (all nans),
- Dissociative Disorder = dissociative_disorders_empty (all nans),
- Substance Use Disorder = substance_abuse_disorders_empty (all nans),
- Addictive Disorder = addictive_disorders_empty (all nans),
- Other = other_disorders_empty (all nans),

    3.2. If possibly, what disorder(s) do you believe you have?

- Anxiety Disorder (Generalized, Social, Phobia, etc).1 = anxiety_disorders_possibly ('Anxiety Disorder (Generalized, Social, Phobia, etc)', nans),
- Mood Disorder (Depression, Bipolar Disorder, etc).1 = mood_disorders_possibly ('Mood Disorder (Depression, Bipolar Disorder, etc)', nans),
- Psychotic Disorder (Schizophrenia, Schizoaffective, etc).1 = psychotic_disorders_possibly (all nans),
- Eating Disorder (Anorexia, Bulimia, etc).1 = eating_disorders_possibly ('Eating Disorder (Anorexia, Bulimia, etc)', nans),
- Attention Deficit Hyperactivity Disorder.1 = adhd_possibly (Attention Deficit Hyperactivity Disorder, nans),
- Personality Disorder (Borderline, Antisocial, Paranoid, etc).1 = personality_disorders_possibly ('Personality Disorder (Borderline, Antisocial, Paranoid, etc)', nans),
- Obsessive-Compulsive Disorder.1 = ocd_possibly (Obsessive-Compulsive Disorder, nans),
- Post-traumatic Stress Disorder = ptsd_possibly (Post-traumatic Stress Disorder, nans),
- Stress Response Syndromes.1 = adjustment_disorder_possibly (Stress Response Syndromes, nans),
- Dissociative Disorder.1 = dissociative_disorder_possibly (Dissociative Disorder, nans),
- Substance Use Disorder.1 = substance_use_disorders_possibly (Substance Use Disorder, nans),
- Addictive Disorder.1 = addictive_disorders_possibly (Addictive Disorder, nans),
- Other.1 = other_disorders_possibly (Asperger, Autism, Suicidal, nans),

    3.3 If so, what disorder(s) were you diagnosed with?

- Anxiety Disorder (Generalized, Social, Phobia, etc).2 = anxiety_disorders ('Anxiety Disorder (Generalized, Social, Phobia, etc)', nans),
- Mood Disorder (Depression, Bipolar Disorder, etc).2 = mood_disorders ('Mood Disorder (Depression, Bipolar Disorder, etc)', nans),
- Psychotic Disorder (Schizophrenia, Schizoaffective, etc).2 = psychotic_disorders ('Psychotic Disorder ('Schizophrenia, Schizoaffective, etc)', nans),
- Eating Disorder (Anorexia, Bulimia, etc).2 = eating_disorders ('Eating Disorder (Anorexia, Bulimia, etc)', nans),
- Attention Deficit Hyperactivity Disorder.2 = adhd (Attention Deficit Hyperactivity Disorder, nans),
- Personality Disorder (Borderline, Antisocial, Paranoid, etc).2 = personality_disorders ('Personality Disorder (Borderline, Antisocial, Paranoid, etc)', nans),
- Obsessive-Compulsive Disorder.2 = ocd (Obsessive-Compulsive Disorder, nans),
- Post-traumatic Stress Disorder.1 = ptsd (Post-traumatic Stress Disorder, nans),
- Stress Response Syndromes.2 = adjustment_disorder (Stress Response Syndromes, nans),
- Dissociative Disorder.2 = dissociative_disorder (Dissociative Disorder, nans),
- Substance Use Disorder.2 = substance_use_disorders (Substance Use Disorder, nans),
- Addictive Disorder.2 = addictive_disorders (Addictive Disorder, nans),
- Other.2 = other_disorders (Depression, Autism, Autism Spectrum Disorder, Depression, Depression, Anxiety, Developmental Trauma, Gender Dysphoria, Panic Disorder, Panic disorder, Tourette's, nans),

4. Mental Health History & Treatment

- Have you had a mental health disorder in the past? = MH_disorder (Yes, No, Possibly, Don't Know),
- Have you ever sought treatment for a mental health disorder from a mental health professional? = sought_treatment (0 = No, 1 = Yes),
- Do you have a family history of mental illness? = family_history (Yes, No, I don't know),
- If you have a mental health disorder, how often do you feel that it interferes with your work when being treated effectively? = work_interference_treatment (Not applicable to me, Sometimes, Rarely, Often, Never),
- If you have a mental health disorder, how often do you feel that it interferes with your work when NOT being treated effectively (i.e., when you are experiencing symptoms)? = work_interference_no_treatment (Not applicable to me, Sometimes, Rarely, Often, Never),
- Have your observations of how another individual who discussed a mental health issue made you less likely to reveal a mental health issue yourself in your current workplace? = observed_neg_impact (Yes, No, Maybe),
- How willing would you be to share with friends and family that you have a mental illness?'= share_with_family (1 - 10 scale),
- Would you be willing to bring up a physical health issue with a potential employer in an interview? = PH_during_interview (Yes, No, Maybe),
- Why or why not? = PH_during_interview_why (various descriptions),
- Would you bring up your mental health with a potential employer in an interview? = MH_during_interview (Yes, No, Maybe),
- Why or why not?.1 = MH_during_interview_why (various descriptions),
- Are you openly identified at work as a person with a mental health issue? = identified_MH (0 = No, 1 = Yes),
- Has being identified as a person with a mental health issue affected your career? = identified_MH_effect (0 = No, 1 = Yes),
- How has it affected your career? = identified_MH_scale (1 - 10 scale) Negative-Positive,
- If they knew you suffered from a mental health disorder, how do you think that team members/co-workers would react? = expected_reaction (1 - 10 scale) Negative-Positive,
- Have you observed or experienced an unsupportive or badly handled response to a mental health issue in your current or previous workplace? = observed_negative_reaction ('No', 'Maybe/Not sure', 'Yes, I observed', 'Yes, I experienced', 'I've always been self-employed'),
- Describe the circumstances of the badly handled or unsupportive response. = describe_negative_reaction (various descriptions),
- Have you observed or experienced supportive or well handled response to a mental health issue in your current or previous workplace? = observed_positive_reaction ('No', 'Maybe/Not sure', 'Yes, I observed', 'Yes, I experienced', 'I've always been self-employed'),
- Describe the circumstances of the supportive or well handled response. = describe_positive_reaction (all nans),
- Overall, how well do you think the tech industry supports employees with mental health issues? = overall_support (Scale 1 - 5),
- Briefly describe what you think the industry as a whole and/or employers could do to improve mental health support for employees. = describe_industry_AOI (various descriptions) areas of improvement,
- If there is anything else you would like to tell us that has not been covered by the survey questions, please use this space to do so. = other_comments,
- Would you be willing to talk to one of us more extensively about your experiences with mental health issues in the tech industry? (Note that all interview responses would be used anonymously and only with your permission.) = followup_talk (0 = No, 1 = Yes),

5. Demographics

- What is your age? = age (various ages),
- What is your gender? = gender (various genders),
- What country do you live in? = country_live (various countries),
- What US state or territory do you live in? = us_state_live (various states, nans),
- What is your race? = race (White, I prefer not to answer, More than one of the above, Asian, Black or African American),
- Other.3 = race_other (Hispanic, Latina, Ashkenazi, European American, Hispanic, White, Indian, Jewish, Latino, Middle Eastern, My race is white, but my ethnicity is Latin American, South Asian, West Indian, mexican american),
- What country do you work in? = country_work (various countries),
- What US state or territory do you <strong>work</strong> in?' = us_state_work (various states, nans),
- Start Date (UTC) = start_date (various dates),
- Submit Date (UTC) = submit_date (various dates),
- Network ID = network_id (unique network id)

<h1>About the project</h1>

Project goals included:
 1. Understand exactly how satisfied tech employees are with mental health issues (Classification, target variable overall_support)
 2. Explore which traits of survey participants and their working environments contribute to this anaysis.
 3. Bring everything above together with data visualizations to describe how these employee traits translate to demographics.

Project Importance:
The tech industry is ever expanding and as more and more people start tech positions the need to understand mental health in this field is extremely important.
Moreover, open-sourcing mental health promotes transparency and can immensely help with sitgma reduction.

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

