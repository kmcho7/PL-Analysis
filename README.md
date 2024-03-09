# Descriptive Analysis of Powerlifting Competition Data and Predicting Max Deadlift of Competitors
 Author: Kevin Cho
 
 Powerlifting meets are held worldwide where competitors attempt their 1 repetition max in the squat, bench, and deadlift. I explored if variables such as gender, age, bodyweight, equipment, and max squat/bench could predict a competitor’s max deadlift. An R-squared value of 0.89 was achieved with linear regression, suggesting reasonable fit and predictive power. Variable selection and Ridge did not improve the prediction performance. The best prediction performance was achieved using Random Forest, a non-linear method. Interesting inferences were made by interpreting the coefficients of the linear regression model. Biological males possibly have a have an advantage over females in deadlift (when all other variables are equal), but this would need to be confirmed by further biomechanical and statistical research.

## Technology

 Data exploration and modeling was done using R and the following libraries:
1. readxl
2. reshape2
3. ggplot2
4. car
5. leaps
6. lars
7. MASS
8. randomForest
9. caret

## Project Files
 1. PL-analysis-report.pdf : A report that discusses the project methodology, results, and conclusion in-depth.
 2. PL-analysis-presentation.pdf : A set of slides that summarize the project report.
 3. PL-analysis-code.Rmd : An R markdown file that contains exploratory data analysis and model training/tuning/testing code.
 4. PL-analysis-code.pdf : A pdf that shows the output of the R markdown code.
 5. openpowerlifting_filtered.xlsx : Filtered version of the OpenPowerlifting dataset from Kaggle containing 89,739 rows x 37 columns with competition data from 1997-2019. Each row represents a competitor (lifter) while the columns represent lifter performance and logstical event information. This dataset will be further processed to remove duplicates and select relevant predictors prior to model building. [https://www.kaggle.com/datasets/caparrini/electronic-music-features-201611-beatporttop100](https://www.kaggle.com/datasets/open-powerlifting/powerlifting-database)
