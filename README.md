# Creating an imputed dataset to create a machine learning model for early stratification of neurological outcomes in cardiac arrest patients. 
#  The overall goal of this project is to create a machine learning model for early stratification of neurological outcomes in cardiac arrest patients. The datasets utilized in this project were two datasets from the international cardiac arrest registry (INTCAR) of Maine Medical Center and a dataset from the electroencephalogram (EEG)-derived indices were used. These datasets contained missing variables that needed to be imputed to continue with the project. This code showcases the process of imputation and analyzing imputation methods. 

# This study aims to develop a dependable model for predicting neurological and cognitive outcomes following cardiac arrest within a critical 6-hour window. Using data from the International Cardiac Arrest Registry (INTCAR) of Maine, the study explores different imputation methods to create a strong dataset for machine learning models. Evaluating three methods—multivariable imputation by chained equations (MICE), k-nearest neighbors (KNN), and mean mode imputation—the study determines MICE as the most accurate. With MICE showing lower Mean Absolute Error (MAE) and higher p-values in statistical tests, it effectively generates a reliable dataset for machine learning applications, enhancing the study's significance.

# procedure: 
# step 1 : Use MICE and KNN to impute the Merged dataset at different levels of missingness. 
Use file 1- 10,20,30% removed data imputed with KNN. This code uses the imputation method KNN to 

file 2 -10,20,30% removed data imputed with MICE: TO TAKE OUT 10,20,30%, SAVE MODIFIED FILE AND IMPUTE WITH MICE: code was used to remove 10% ,20% ,30% for known data and then it was imputed using MICE method of imputation.

# step 2: evaluate the imputed data.we used 4 different tests : KS test, T test ,MAE and fractional error to evaluate the data imputation methods.They were all compared with mean and mode as a control
file 3:KS T test - KNN & MICE : TO CALCULATE KS&T TEST, SUMMARY STATISTICS : code was used to evaluate the KNN and mice imputation by calculating the KS test and T test.

file 4:MAE and normalized fractional error KNN & MICE : TO CALCULATE MAE AND NORMALIZED FRACTIONAL ERROR : code was used to evaluate the KNN and MICE imputation by calculating the MAE and normalised fractional error.

file 5 :Overall MAE- KNN & Mice: Calculate overall MAE for KNN and MICE : code used to calculate the overall MAE for MICe and KNN imputaion methods.

# step 3 : visualisation of data.the results were visualised using KDE plots for numerical variables ,bar plots for binary and categorical variables .Mean/mode was used a control to compare.

file 6: KDE plots for numerical values- KNN & MICE : TO CREATE KDE PLOTS FOR NUMERICAL VARIABLES : code was used to visualise the numerical values by using KDE plots.The data was imputed using both Mice and KNN and compared with the original data.The variables shown : BISi', 'SRi', 'BIS6', 'SR6', 'ABGpH', 'age',etc.

File 7: Bar graphs - categorical data -KNN & Mice : BAR GRAPHS FOR CATEGORICAL: code was used to visualise the categorical values using bar plots.The data was imputed using both Mice and KNN and compared with the original data.The variables shown : 'echoWithin12','glasgow','rankinPrior', 'CPCprior', 'hospCondition',etc.

File 8: Bar graphs - binary variables -KNN & Mice : BAR GRAPHS FOR BINARY :code was used to visualise the binary values using bar plots.The data was imputed using both Mice and KNN and compared with the original data.The variables shown : 'ambulate', 'aorticBalloon', 'arrythmia', 'BIS','cervascD', 'civilianCPR', 'civilianDefib', 'cogImpair', 'contissD',etc.

# file name with descriptions : short description: long description 
1)10,20,30% removed data imputed with KNN : TO TAKE OUT 10,20,30%, SAVE MODIFIED FILE AND IMPUTE WITH KNN: code was used to remove 10% ,20% ,30% for known data and then it was imputed using KNN method of imputation.

2)10,20,30% removed data imputed with mice : TO TAKE OUT 10,20,30%, SAVE MODIFIED FILE AND IMPUTE WITH MICE: code was used to remove 10% ,20% ,30% for known data and then it was imputed using MICE method of imputation.

3) KS T test - KNN : TO CALCULATE KS&T TEST, SUMMARY STATISTICS : code was used to evaluate the KNN and MICE imputation by calculating the KS test and T test.
  
4) MAE and normalized fractional error KNN : TO CALCULATE MAE AND NORMALIZED FRACTIONAL ERROR : code was used to evaluate the KNN and mice imputation by calculating the MAE and normalised fractional error.
   
5)Overall MAE- KNN & Mice: Calculate overall MAE for KNN : code used to calculate the overall MAE for MICe and KNN imputaion methods 

6) KDE plots for numerical values- KNN & MICE : TO CREATE KDE PLOTS FOR NUMERICAL VARIABLES : code was used to visualise the numerical values by using KDE plots.The data was imputed using both Mice and KNN and compared with the original data.The variables shown : BISi', 'SRi', 'BIS6', 'SR6', 'ABGpH', 'age', 'glucAdm', 'HCO3Adm', 'height', 'lactateAdm',etc.
   
7) Bar graphs - categorical data -KNN & Mice : BAR GRAPHS FOR CATEGORICAL: code was used to visualise the categorical values using bar plots.The data was imputed using both Mice and KNN and compared with the original data.The variables shown : 'echoWithin12','glasgow','rankinPrior', 'CPCprior',Etc.

8) Bar graphs - binary variables -KNN & Mice : BAR GRAPHS FOR BINARY :code was used to visualise the binary values using bar plots.The data was imputed using both Mice and KNN and compared with the original data.The variables shown : 'ambulate', 'aorticBalloon', 'arrythmia', 'BIS','cervascD', 'civilianCPR', 'civilianDefib', 'cogImpair', 'contissD',etc.

