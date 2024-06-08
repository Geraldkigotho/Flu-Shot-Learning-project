# A Flu-Shot MachineLearning project

![image](https://github.com/Geraldkigotho/Flu-Shot-Learning-project/assets/162441488/2b506e8a-73e2-4a6a-9942-b8712d3857c6)


### BUSINESS UNDERSTANDING

**OVERVIEW**

Vaccines play a very crucial role in disease prevention, they work by providing immunity to individuals as well communities to prevent specific communicable diseases like COVID-19, swine flu, influenza and Tuberculosis. The first vaccine was developed in 1796, by an English physician Edward Jenner and was used to vaccinate the first human against smallpox. Today’s vaccines have evolved and become more complex, robust and more efficient these is due to the continuous growth of technology and research in the health industry. Hence measures have been put in place to ascertain quality, efficiency and distribution of the vaccines. The H1N1 VACCINE was developed in 2009 and approved for use in 2010  after the swine flu pandemic broke out in 2009 killing more than two million people worldwide while the seasonal vaccine also known as the 'flu-shot' is commonly used to prevent flu (influenza) during the flu season.

The Center for Disease Control and Prevention (CDC) wants to understand how different individual personal characteristics influence the uptake of the H1N1 and seasonal vaccine as well as the vaccine patterns which would provide guidance for future public health efforts.

**PROBLEM STATEMENT** 

Vaccines are critical for preventing communicable diseases such as COVID-19, swine flu, seasonal influenza, and tuberculosis. However, making data-driven decisions about vaccine distribution and delivery remains difficult. The CDC seeks to understand how individual features influence uptake of the vaccines so as to provide guidance for future public health efforts

**OBJECTIVES** 

**Main Objectives**

.To predict how likely people are to get the H1N1 and seasonal flu vaccines.


**Specific Objectives**

.To determine the distribution of the uptake of the H1N1 and seasonal vaccines

.To determine the correlation between the uptake of both vaccines

.To determine which characteristics are likely to influence one to taking a particular vaccine


### DATA UNDERSTANDING

**DATA SOURCE**

Data was downloaded from https://www.drivendata.org/competitions/66/flu-shot-learning/data/ which a phone survey was done in 2009 courtesy of the United states National Center for Health Statistics

**DATA DESCRIPTION**

**Features**

These data set contained  features to be used for predicting our target variable

These features are sourced from respondents reply during the phone survey

**Labels**

These data set contain our target variables H1N1 and seasonal vaccine take encoded in binary form [0,1]

### DATA PREPARATION

Steps that were used to clean the data

. **Completeness** (we will check for missing values , how they affect our data set and how we will handle them)

. **Consistency** (we will check for duplicate values and how to handle them)

. **Uniformity** (we will check for uniformity in column data types)

. **Validity** (we will handlle irrelevant columns and check for outliers )

### DATA ANALYSIS

#### Univarent analysis

**Vaccine Distribution**

![image](https://github.com/Geraldkigotho/Flu-Shot-Learning-project/assets/162441488/9b100e00-5efc-4d1c-9158-863330cd62de)

**Observation** many people opt to take the seasonal vaccine compared to the H1N1 vaccine and also there seems to be a class imbalance in the H1N1 class which we will correct later on

#### Bivarent analysis

Comparing categorical variables with our target variables 

**Gender distribution according to uptake of vaccines**

![image](https://github.com/Geraldkigotho/Flu-Shot-Learning-project/assets/162441488/3e19df16-3b09-4b80-86b4-f5f8078fec25)

**Observation** Seems most of the people who are taking vaccines are of the female gender, these could be a area to research on as to why men are not getting vaccinated

### MODELLING

We created 5 models and evaluated them to find the best fitting models for our target variables

|MODEL	           |ACCURACY H1N1	|ACCURACY SEASONAL|	AUC H1N1 |AUC SEASONAL|
|------------------|----------------|-----------------|----------|------------|
|Decision tree     |	0.59        |  0.67	          |0.6	     |0.68        |
|Logisticregression|	0.82        |    	0.78	  |0.64	     |0.78        |
|KNN	           |    0.63        | 	0.71	      |0.64	     |0.71        |
|Naïve Bayes	   |    0.65        |	0.74	      |0.69	     |0.74        |
|Random Forest     |	0.63	    |0.77	          |0.65	     |0.78        |
|Tuned KNN	       |	0.83	    |0.78             |0.65	     |0.77        |

**Evaluation**

**Classfication metric used and why ?** 

AUC measures the model specificity and sensitivity hence it measures the model ability to distinguish between postive and negative in imbbalanced data while accuracy score is easy to understand and interprate.

**Models choosen and their observations**

With an AUC score of 0.65 and  an accuracy of 0.83, the Tuned KNN model is the best  model for predicting the "h1n1" class while  the logistic regression model is the best option for predicting the "seasonal" class because it has an accuracy of 0.78 and AUC score of 0.78

**CONCLUSIONS**

Majority of the respondents have been vaccinated with seasonal vaccine more than h1n1 vaccine

Majority of the respondents who have been vaccinated are of female gender

Majority of the respondents who have been vaccinated are 55 year old and above

Majority of the respondents who have been vaccinated have a higher education level most of them had graduated from college

**RECOMMEDATIONS**

. Targeted Vaccination programs: creating vaccination programs that targets the groups such as females, people aged 55 and over,   higher education students and high income earners..

. Addressing Racial discrepancies: While most of the vaccinated respondents were  white, other racial groups should be also monitored to prevent or stop any racial discrepanicies through public 
  education and awareness campaigns and vaccination drives that target at all the ethnic groups to ensure those of color get equal access to the vaccines.


  **My Repository breakdown**

  The vaccine data folder contains two Excel dataset features and a label

  







