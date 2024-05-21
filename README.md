# Analysis of Smoking Insurers

## Project Overview

This project aims to unpack the impact of smoking on insurance charges and the rate of smoking between men and women.
Since we are testing the means of two samples (smoking and non-smokers) for inferential statistics, we employed a t.test method.

## Data Sources

A csv insurance data from kaggle website was used. The dataset contained variables are ;
- age - Age of the insurer
- sex - Sex of the insurer
- bmi - The body mass index
- children - The number of children the insurer have
- smoker - Does the insurer smoke?
- region - From which region is the Insurer from?
- charges - Insurance charges

## Tools/Packages

All data cleaning steps and analysis were done inside R-studio using R-markdown format. The following packages were used for the analysis;
- readr
- tidyverse
- dplyr
- Hmisc
- mice
- summaryTools

## Data Cleaning/Preparation

The data cleaning and preparation phase included the following steps;
- Checked for missing values and found none
- Recoded the smoker variable from "yes" and "no" to "1" and "2" responses
- Created a smoker_dummy variable where smoker response was 2

## Data analysis
- Calculated the smoking rate by summing the smoker_dummy variable and deviding by the number of rows and multiplied by 100.
- Hypothesis testing of social media claims

## Results and Findings

- The smoking Rate was 20.49%

- For the Claim: **Insurers who smoke are charged more than insurers who does not smoke**. The mean charge for smoking insurers was 32050.23 while that of non_smokers was 8434.268.
The t.test also revield the same mean charge values for the two groups. The test revieled that there is a 95% chance that the difference in charge between the smokers and non-smokers is from 22197.21 to 25034.71. So, on average, an insurer who smoke is charged higher than an insurer who does not smoke. The p-value of 2.2e-16 suggest that we reject the null hypothesis and accept the alternative hypothesis that insurers who smoke are charged higher than insurers who do not smoke.

- For the claim: **There is no relationship between sex and smoking**. Male insurers have 23.5% smoking rate while woman insurers have 17.4% smoking rate. The t.test revieled the same mean smoking rate between the insurer sexes. The test also unpacked that we are 95% confident that male insurers have from 1.8 to 10% higher smoking rate than female insurers. With p-value = 0.005248, we accept the null hypothesis and conclude that indeed male insures have higher smoking rate than female insurers.

See analysis report (https://raw.githack.com/Celumusa91/Analysis-of-smoking-in-insurance-data/main/Hypothesis-Testing-script.html)

See analysis code (https://raw.githubusercontent.com/Celumusa91/Analysis-of-smoking-in-insurance-data/main/Hypothesis%20Testing%20script.Rmd)

