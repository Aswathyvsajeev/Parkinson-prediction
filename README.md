# Parkinson-prediction #

## What is Parkinson's Disease? 
Parkinson’s disease is a chronic disease condition which affects parts of the brain and leads to damage of nerve cells.Tremor,stiffness and lack of flexibility are the main symptoms of Parkinson’s disease.It can also lead to psychological problems like depression and anxiety. Men have more chance of having Parkinson’s disease compared to women. According to 2020 statistics UK,around 145,000 people have Parkinson’s disease and is estimated to rise around 172,000 by 2030.

## Project Overview 
- Different machine learning classifiers are developed with the goal of distinguishing people with Parkinson’s disease from healthy ones using dysphonia measures collected from    patients 
- Performance of the models are compared to identify which model performs best. Support vector machine and K-Nearest Neighbor are compared to Artificial neural network 
 model. 
- Artificial neural network is built using Keras library in python 
- The dataset is collected from UCI repository.
- To evaluate the performance of the models K-fold cross validation is used.In addition to that, for evaluating the model different performance matrices like confusion matrix,    sensitivity, precision, specificity, recall and F1 score are used.

## Code And Resources Used
Python Version-3.7.11

Packages: numpy,pandas,matplotlib,seaborn,tensorflow,sklearn,keras

Dataset: http://archive.ics.uci.edu/ml//datasets/Parkinsons

## EDA

Explored the data and identified the correlation of the variables using heatmap.

![image](https://user-images.githubusercontent.com/88787271/131018109-00ee4b0c-9ea0-4312-a1e9-7c3f36927ef7.png)

Below barchart shows the count of people with parkinson's disease and withoout disease.

![image](https://user-images.githubusercontent.com/88787271/131018467-830389e8-a721-4413-a66b-303ea8174de2.png)

pairplot is used to identify the pairwise relationship in the dataset.

![image](https://user-images.githubusercontent.com/88787271/131018985-3ed7f8e3-a080-44dd-9550-24a72706c403.png)

## Model Building
The dataset does not have any missing data. All the observations in the dataset are used in this study.Feature scaling is used to scale the data,since the feature variables are in different scales.Standardization method is used for feature scaling with the help of built-in standard scaler. It guarantees that each feature has a mean of 0 and variance of 1.From the dataset,75% of the data is used for training the model and 25% of the data is used for testing the model.In the dataset,‘Status’ attribute is used as the dependent variable and all other attributes are used as feature variables.

Below 3 models are used and their performance is evaluated:
- Artificial Neural Network
- Support vector machine
- K Nearest Neighbor

## Evaluation

The three model are compared based on different performance matrices .Artificial neural network outperformed the other models in terms of all the performance metrics with 
93.14% accuracy,100% recall,94.87% precision and 97.36% F1 score.100% recall shows that the model can detect all the individuals with Parkinson’s disease and that make the model a very good fit.




