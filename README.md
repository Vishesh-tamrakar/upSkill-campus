# Upskill_Quality_Prediction

# Project Title : Quality Prediction in a Mining Process
/ submitted to Upskill Campus /

### Links to Dataset :


Github link - https://github.com/Vishesh-tamrakar/Upskill_Quality_Prediction/blob/main/MiningProcess_Flotation_Plant_Database.csv

Google Drive link - https://drive.google.com/file/d/1mZl1j2m_YiLFCSvduw0MpsBPkgJy396y/view

### Links to Code :

Github link - https://github.com/Vishesh-tamrakar/Upskill_Quality_Prediction/blob/main/UpSkill_Project.ipynb

Google Colab link - https://colab.research.google.com/github/Vishesh-tamrakar/Upskill_Quality_Prediction/blob/main/UpSkill_Project.ipynb#scrollTo=s4sN-8bEtbbA

## CONTEXT

With the help of the provided dataset from a flotation plant of a mining plant our main goal is to use this data to predict how much impurity is in the ore concentrate. As this impurity is measured every hour, if we can predict how much silica (impurity) is in the ore concentrate, we can help the engineers, giving them early information to take actions. Hence, they will be able to take corrective actions in advance (reduce impurity, if it is the case) and also help the environment (reducing the amount of ore that goes to tailings with the reduce of silica in the ore concentrate).

Hence We decided to work upon this Industrial manufacturing and production problem by using machine learning algorithms to perform the necessary predictions. 

## DATASET INFORMATION

The dataset was obtained from a mineral processing plant separating silica from iron ore using the reverse cationic flotation method. Continuous process data were collected from 1 a.m. on March 10, 2017 to 11 p.m. on September 9, 2017.

Each row of data consists of 23 measurements that can be categorized into four types:

●	raw materials (column 2-3);

●	environment variables (column 4-8);

●	process variables (column 9-22);

●	processed materials (column 23-24).

Raw materials and processed materials were sampled on an hourly basis while the others were sampled every 20 second.

The first column shows time and date range (from march of 2017 until september of 2017).he second and third columns are quality measures of the iron ore pulp right before it is fed into the flotation plant. Column 4 until column 8 are the most important variables that impact the ore quality at the end of the process. From column 9 until column 22, we can see process data (level and air flow inside the flotation columns, which also impact ore quality. The last two columns are the final iron ore pulp quality measurement from the lab.

## INFERENCES FORMED

-> % SILICA CONCENTRATION FORECAST TIME CALCULATION

-> PREDICTION OF % SILICA CONCENTRATE WITH AND WITHOUT USING % IRON CONCENTRATE COLUMN

## CONCLUSION

Deep learning approach using LSTM was implemented to forecast gangue content in flotation concentrate.

Excluding % iron in concentrate from the features, % silica in concentrate were forecasted one hour ahead and with error below 1 (based on RMSE, MAE). As per the dataset MAE and RMSE of 1±0.2 is a satisfactory result. The forecasts thus show a promising method for the engineers to make timely assessments of concentrate purity and take corrective actions in advance, especially when purity deviates from the acceptable values.

Hence Yes, It is possible to predict % Silica in Concentrate without using % Iron Concentrate column.
But here we also observe that the R^2 value with inclusion of % Iron Concentrate column is greater that when not included that means it did really helped in the prediction because of the high correlation between them .
