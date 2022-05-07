# MLFA-Spring-2021-22
This repo has all the assignment solutions for the course AI60002, Spring Semester 2021-22 taught at IIT Kharagpur. 



<h3>The question for assignment 5 is stated below:</h3>

Download the attached dataset called “S_n_I_A_N_P_An_Io_noaa2.txt”. The dataset contains 870 rows × 7 columns in a space separated manner. The columns are ‘SAM’, ‘nino’, ‘ISMR’, ‘AMO’, ‘NAO’, ‘PDO’, ‘At-nino’, ’IOD’. Here ISMR is mean monthly rainfall in Indian region. Other columns denote potential causal drivers for ISMR, which are climatic conditions in other parts of the world. The rows contain monthly data for the months ‘May’, ‘June’, ‘July’, ‘Aug’, ‘Sep’, ‘Oct’ for the years 1871-2015 (145x6=870).  E.g., The first row contains the data for May, 1871. Ignore the column "SAM".

ISMR can be predicted using the potential drivers, but the lags can be different. E.g., If rainfall of July is caused by the driver values of May, then the lag value will be 2. That means the predictor values of 2 months back causes the rainfall of the current month. Use ‘Xgboost regresssor’ to predict ISMR for different lag values of the drivers and print the true and predicted values of the ISMR for different lags in a tabular form.

Plot the true values vs predicted values of ISMR in scatter plots for different lags separately. Find out which lag is statistically showing best result and elaborate why.

Repeat the experiment (2,3) for SVM with different kernel values to find the best performing one. Use grid search method to find the best performance.[S_n_I_A_N_P_An_Io_noaa2.txt](https://github.com/Ayushman-0301/MLFA-Spring-2021-22/files/8645058/S_n_I_A_N_P_An_Io_noaa2.txt)


<h3>The question for assignment 6 is stated below:</h3>
Download the attached dataset ‘Twitter_data.csv’. The dataset contains the usage data of twitter along with the days of the week (Friday-Sunday). The columns present in the dataset are ‘TweetID’, ‘Day’, ‘Hour’, ‘Lang’, ‘IsReshare’, ‘Reach’, ‘RetweetCount’, ‘Likes’, ‘Sentiment’, ‘text’, ‘LocationID’, ’UserID’. All the columns are self-explanatory. We will use the data to cluster them according to the days of a week. 

Check for any missing values in the dataset. If there, drop the rows. 

Drop any redundant column. (If you feel it is needed) 

Separate the target column(‘Day’) from the dataset and convert it from categorical to integer. 

Visualize the dendogram of the data. 

Implement Hierarchical Agglomerative clustering with single and complete linkage both to cluster the dataset. You have to write the code from scratch without using any package for the clustering method. You can use general packages like numpy, pandas, matplotlib etc. 

Plot the resultant clusters in scatter plot. 

Report the percentage accuracy of the clustering. 
[Twitter_data.csv](https://github.com/Ayushman-0301/MLFA-Spring-2021-22/files/8645067/Twitter_data.csv)


<h3>The question for assignment 7 is stated below:</h3>
Features need to be considered: na_value = ‘?’

age: age in years
sex: sex (1 = male; 0 = female)
cp: chest pain type
– 1: typical angina
– 2: atypical angina
– 3: non-anginal pain
– 4: asymptomatic
trestbps: resting blood pressure (in mm Hg on admission to the hospital)
chol: serum cholesterol in mg/dl
fbs: (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)
restecg: resting electrocardiographic results
– 0: normal
– 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)
– 2: showing probable or definite left ventricular hypertrophy by Estes’ criteria
thalach: maximum heart rate achieved
exang: exercise-induced angina (1 = yes; 0 = no)
oldpeak: ST depression induced by exercise relative to rest

Using this data implement following regression techniques from scratch without using any library function.

Linear Regression
Lasso Regression
Ridge Regression

[data.csv](https://github.com/Ayushman-0301/MLFA-Spring-2021-22/files/8645071/data.csv)
