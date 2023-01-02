# Cardiovascular-Risk-Prediction

PROBLEM STATEMENT

The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides, the patients' information. It includes over 4,000 records and 15 attributes. Each attribute is a potential risk factor. There are both demographic, behavioral and medical risk factors.


Approaches:-

**Step 1** - Viewing and cleaning data being the initials, we started with importing necessary libraries, mounting drive and storing data in variables for deriving meaningful insights. 

![COLUMNS](https://user-images.githubusercontent.com/112775752/210253638-ae397c65-9e73-43c7-8e8e-18348235e754.png)

![DESCRIBE](https://user-images.githubusercontent.com/112775752/210253652-0f4af5f1-ee57-4b8b-943d-05d4fd28863f.png)

Next step being data analysis and visualization, where we analyzed our data distribution as univariate, bivariate and multivariate plots. Multicollinearity check was performed.

![BP MEDS](https://user-images.githubusercontent.com/112775752/210253696-88d8f995-29d5-4c78-b4cb-2fc8cd84b2bc.png)

![DIABETES](https://user-images.githubusercontent.com/112775752/210253716-1ad35467-e920-47c7-b085-93916ca79d13.png)

![GENDER](https://user-images.githubusercontent.com/112775752/210253729-616fd972-6dc1-4e0d-be7b-be5c0d02e0f3.png)

![SYSDIAS](https://user-images.githubusercontent.com/112775752/210253786-a0fde639-f930-492b-af0b-79148d118276.png)

![HEATMAP](https://user-images.githubusercontent.com/112775752/210253816-7080d2f9-3850-4469-84e9-35a3dc837b72.png)

**Step 2** - We performed 3 hypothesis testing one was presence of outliers using boxplots, second was asssociation of age and cardiovascular risk using chi_square test, last was mean value of total cholesterol using z test

**Step 3** - Presence of null values would have created possible errors in the further steps, so we replaced numerical null values with median, as median is unaffected by outliers and categorical null values are replaced by mode. We also removed outliers which were irrelevant, as all outliers cannot be removed or replaced due to thier importance in risk prediction.

**Step 4** - As a part of feature engineering we added a new column BP using systolic and diastolic bp which were found to be highly correlated. Also cigsperday column was converted to categorical column. then we performed hot encoding to create dummy variables for categorical data, our data was highly imbalanced so we used SMOTE to create a balanced data.

![IMBALACE](https://user-images.githubusercontent.com/112775752/210253845-e9516403-5ca5-4725-b958-78702ebac7ef.png)

**Step 5** - Last step was to perform model training using different algorithms, we tried logistic regression, KNN, Naive-Bayes, XGBclassifier, Random Forest. Evaluation metrics used for comparing models were f1 score and recall.

BEST MODEL

KNN

![KNN](https://user-images.githubusercontent.com/112775752/210254086-d7e5ffb5-790c-4d1f-aaf0-b26e3cbefc6c.png)

CONCLUSION:

## EDA :- 
*  Our data set has 17 features & 3390 rows. We studied all these features and have drawn following comclusions:
 
  * The very first graphs gives us the distribution of dependent variable and whch shows that very less no of peoples are prone to cardiovascular risk.
  
  * Any value outiside the given normal range determines higher risk of cardiovascular risk. Thus, various companies like insurance, healthcare, fitness-nutrition and medical can target this population for better revenue generation.

  * We have observed that people wether or not smoking are at equal risk of cardio vascular diseases, which suggests companies to target them equally.
  * Our data shows that people having hypertension are more prone to cardio vascular diseases, very less no. of paitents are on BpMeds, but 50 % of then are at cardiovascular risk, which is significant. Thus, this information can be leveraged by various companies. 
  * Distribution of cardiovascular Risk and Age shows that with increase in age chances of having cardiovascular diseases increases.
  * Diabetic patients are high risk of getting cardio vascular disease as our data shows; ~ 61% of the diabetic population is at high risk.
  * Gender distribution shows that males are more prone to cardio vascular risk as compared to females because the frequency of males having smoking habits is more.
  * Another bivariate plot between Systolic and diastolic BP shows that they are positivly correalted and with increase in any of this values increses the ridk of cardiovascular diseases.
  * Orderwise correlation shows that age and systolic pressure highly affect our dependent variable.








