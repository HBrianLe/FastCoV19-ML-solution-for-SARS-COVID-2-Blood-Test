![FASTCoV19](https://github.com/andytrcs/FastCoV19/blob/main/Project_Title.png)
# FastCoV19-ML-solution-for-SARS-COVID-2-Blood-Test
This work has the objective to predict confirmed COVID-19 cases among suspected cases based on commonly collected laboratory exams.
## Objectives
This work has the objective to predict confirmed COVID-19 cases among suspected cases based on commonly
collected laboratory exams.
We consider the following question:
Based on the results of laboratory tests commonly collected for a suspected COVID-19 case during an annual
physical exam, would it be possible to predict the test result for SARS-Cov-2 (positive/negative)?
## Data Set
The dataset contains anonymized data from patients seen at the Hospital Israelita Albert Einstein in São
Paulo, Brazil, and who had samples collected to perform the SARS-CoV-2 RT-PCR and additional laboratory
tests during a visit to the hospital.
## Data Preparation
- Data cleaning procedures:
1. Make variable names syntactically valid by removing special characters, spaces and symbols
2. Convert strings that represent missing data to NA, namely the following values: ‘Não Realizado’ and
‘not_done’
3. Convert string categorical values to factors
4. Convert the variable Urine. . . pH to numeric, as it contains a mix of string and numeric values in the
input data
