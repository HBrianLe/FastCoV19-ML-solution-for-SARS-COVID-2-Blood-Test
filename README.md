# FastCoV19-ML-solution-for-SARS-COVID-2-Blood-Test
![FASTCoV19](https://github.com/andytrcs/FastCoV19/blob/main/Project_Title.png)
This work has the objective to predict confirmed COVID-19 cases among suspected cases based on commonly collected laboratory exams.

## Objectives
This project is aim to predict confirmed COVID-19 casess based on laboratory result from anual physical
exams.
We consider whether it be possible to predict the test result for COVID 19 (either positive or negative) based
on the result of blood test?

## Data Set
We retrieve the dataset from patients seen at the Hospital Israelita Albert Einstein in São Paulo, Brazil,who
perform the COVID 19 test and additional laboratory tests.
The dataset contains 109 variables (predictors), a Patient ID and one target outcome variable, which indicates
whether the patient tested positive/negative for SARS-Cov-2.
This dataset has 109 variables, a Patient ID and one target outcome variable showing the result (positive/
negative) of COVID 19.

## Data Cleaning
Data cleaning procedures consist of: Making variable names syntactically valid, Replacing column values
that should be empty for NA, Convert string categorical values to factors, Convert the variable Urine. . .pH
to integer
The outcome variable SARS.Cov.2.exam.result is a binary by which we convert such that
SARS.Cov.2.exam.result = 1 for being positive and SARS.Cov.2.exam.result = 0 for being negative
with COVID 19.
However, there are too many missing data points (>= 95%); we decided to remove them along with poor
sample. But we choose to keep negative samples that have at least 10 variables with data points available.

## Predictive Analysis
Model Training
To predict the likelihood that a patient is infected with the COVID 19, we split the dataset randomly into
training and testing tests in a train-to-test split ratio of 4/5.
