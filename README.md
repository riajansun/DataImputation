# Creating an imputed dataset to create a machine learning model for early stratification of neurological outcomes in cardiac arrest patients. 
#  The overall goal of this project is to create a machine learning model for early stratification of neurological outcomes in cardiac arrest patients. The datasets utilized in this project were two datasets from the international cardiac arrest registry (INTCAR) of Maine Medical Center and a dataset from the electroencephalogram (EEG)-derived indices were used. These datasets contained missing variables that needed to be imputed to continue with the project. This code showcases the process of imputation and analyzing imputation methods. Through evaluation, MICE emerges as the most accurate method, exhibiting lower Mean Absolute Error (MAE) and higher p-values in statistical tests. This finding underscores MICE's effectiveness in generating reliable datasets for machine learning applications, thus enhancing the study's overall significance in predicting neurological and cognitive outcomes post-cardiac arrest within a critical 6-hour window. This README is description of the processes used to get to the final conclusion. 

# procedure: 
# step 1 : Use MICE and KNN to impute the Merged dataset at different levels of missingness. 
Use file 1- 10,20,30% removed data imputed with KNN. This code first removes 10%, 20%, and 30% of known variables, saves the modified files and then imputes with KNN, with k=5. 

use file 2 -10,20,30% removed data imputed with MICE.  This code first removes 10%, 20%, and 30% of known variables, saves the modified files and then imputes with MICE in R studio.

file 3 - Mean mode imputation(control). This code first removes 10% of known variables, saves the modified file and then imputes with Mean/Mode. It was used as a control 

# step 2: evaluate the imputed data using KS test, T test, MAE, and normalized fractional error. 

file 4: KS T test - KNN & MICE : The code was used to  evaluate the KNN and mice imputation by calculating the KS test and T test.

file 5: MAE and normalized fractional error KNN & MICE : This code was used to evaluate the KNN and MICE imputation by calculating the MAE and normalised fractional error.

file 6 :Overall MAE- KNN & Mice: This code was used to calculate the overall MAE for MICe and KNN imputaion methods.

# step 3 : visualisation of data.the results were visualised using KDE plots for numerical variables ,bar plots for binary and categorical variables .Mean/mode was used a control to compare.

file 7: KDE plots for numerical values- KNN & MICE :This code was used to visualise the numerical values by using KDE plots.The data was imputed using both Mice and KNN and compared with the original data.The variables shown : BISi', 'SRi', 'BIS6', 'SR6', 'ABGpH', 'age',etc.

File 8: Bar graphs - categorical data -KNN & Mice : This code was used to visualise the categorical values using bar plots.The data was imputed using both Mice and KNN and compared with the original data.The variables shown : 'echoWithin12','glasgow','rankinPrior', 'CPCprior', 'hospCondition',etc.

File 9: Bar graphs - binary variables -KNN & Mice : This code was used to visualise the binary values using bar plots.The data was imputed using both Mice and KNN and compared with the original data.The variables shown : 'ambulate', 'aorticBalloon', 'arrythmia', 'BIS','cervascD', 'civilianCPR', 'civilianDefib', 'cogImpair', 'contissD',etc.



