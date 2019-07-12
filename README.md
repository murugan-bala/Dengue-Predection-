# Dengue-Predection-
Dengue prediction  using Raspberry pi Board :

DATA COLLECTIONS:

The prediction of Dengue Fever is going to done by getting the Datasets from different States from india 
The datasets contains information about number of dengue cases observed every month for 2018 years in many number of states
It contains details about the dengue symptomes  like Fever, Temperature , Fatigue ,Vomiting  and so on. Dataset by using 

Logistic Regression

  DATA PREPROCESSING:


1. Missing Values

	Missing values leads to improper learning, Missing values can be handled in two ways,
i) Removal of Data instances: The data instance which has missing value for any feature was removed. In this way we removed the unreliable data point from the training set but at the same time we have reduced the dataset size from 5000 to 1000.
ii) Filling the missing values: The missing values in the data point were assigned the most frequently occurring value for that feature. We have used the package “preprocessing” and the functionality “Imputer()” from scikits. learn. We observed that using the second approach (i.e. Imputer) the results were more accurate.
2. Standardization
	There can be huge variation in the values of a feature over the entire dataset. This will make it difficult for the model to learn the data properly. This makes it necessary to standardize the data. • We have implemented this by removing the mean from the value of each feature and scaling to unit variance. For this purpose we have used the functionality “Standardscalar()” from the pre-processing package.
3. nominal values
	The feature “states” in the dataset contains the names of three states. We need to convert character values to numerical value. We have implemented the same by using LableEncoder() functionality of the preprocessing package.

LEARNING MODELS
For predicting the data, the Logistic regression  algorithm (LRA) is used, and in LRA we are using Sigmoid Technique.
 An sigmoid is just a collection of predictors which come together (e.g. mean of all predictions) to give a final prediction.
 Further, Mean Square Error (MSE) gives the difference between the existing and proposed data, (i.e. MSE can represent the difference between the actual observations and the observation values predicted by the model.
Mean Square Error (MSE), we have to find the pattern and dependencies in the given training dataset and predict number of dengue cases for the given week and year of a  states in the test dataset.



INTERGRATION OF RASPBERRY PI:

We intergrating raspberry pi with machine learning concept . We run code on raspberry pi 3 :

Specification :

Model: Raspberry pi – 3 Model B+

Processor: Broadcom(BCM 2837)

Software: Raspbian OS

Language : C,C++,Java, Python(recommended)

Power supply: maximum 5V(up to 2Amps)
