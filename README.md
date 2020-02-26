# crime-type-data-exploration

## Background
Crime is a social problem faced by many countries around the world. Other than affecting the citizens’ quality of life, criminal activities can incur large amount of cost on the country (law enforcement, maintenance of prisons, prosecution). To overcome this issue, the field of computing has made remarkable advances in using machine learning to aid crime prevention such as a recent one conducted by Ahishakive, Omulo, and Niyonzima (2017). Nonetheless, most of the studies conducted have focused primarily on predicting probability of crime occurrence without classifying the type of crime (Murad, Mustapha, and Khanahmadliravi, 2013). Moreover, valuable information such as the characteristics of the criminals or victims that can help predict crime are difficult to obtain due to ethical reasons. Therefore, the purpose of this project is to make use of the available data such as location and time to build a machine learning model that can predict the type of crime and its’ respective probability of occurring in different areas.  

## Overview of dataset
This dataset is obtained from UK police website (URL: https://data.police.uk/data/) from June 2019 to July 2019. In several areas in UK, this dataset contains all crime data recorded within the respective police database in each area. Each crime data from different area is generated separately so data from different areas are combined into one file containing 12 variables and 1141086 observations.  

![rex](data-exploration-1.png)

With plot intro command, an overview of the dataset is produced as shown as above, 75% of the dataset is discrete columns while 16.7% of the dataset is continuous columns. 

## Features in dataset
Below is the list of features in the dataset.
![rex](data-exploration-2.png)

## Bar plot for discrete variables
![rex](data-exploration-3.png)
![rex](data-exploration-4.png)

Based on the bar plot above, vast majority of the crime are reported by Metropolitan police service, which also falls within the jurisdiction of Metropolitan police service. Nonetheless, the number of stations and population that is under jurisdiction of Metropolitan police service is much higher than the other area, hence the much higher crime rate.

![rex](data-exploration-5.png)

Among all the type of crimes, violence and sexual offences are the most common type of crime followed by anti-social behaviour.
Based on the initial analyses above, the dataset provides large amount of information but also contains several issues that may require further treatment to optimize the performance of the machine learning algorithms. The large number of categorical data will require encoding to be conducted. For the purpose of this dataset, one-hot encoding may be appropriate given the large number of categories in each variable. 
Furthermore, the class imbalance in the reported by and crime type columns also pose challenge to the algorithms as well. This may suggest that conventional metrics used to evaluate machine learning algorithms may not be applicable for this dataset. In this case, resampling or using a different evaluation metrics will be considered. 
