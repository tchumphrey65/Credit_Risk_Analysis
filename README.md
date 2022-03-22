
![image](https://user-images.githubusercontent.com/91839403/159567507-5f547544-70b3-4ab0-8797-e95295cec44c.png)



# Credit_Risk_Analysis

## Project Overview

The goal of this project is to use a dataset from LendingClub to evaluate and compare machine learning models.  The expectation is that this analysis will evaluate and compare several machine learning approaches to determine the best approach to predicting credit risk 

The approaches we have been tasked with evaluating are:

1) Oversampling with Ramdom Oversampler and SMOTE machine learning algorithms.
2) Undersampling with the ClusterCentroids algorithm.   
3) Over/Under Sampling Combinatorialusing the SMOTEENN algothrim.
4) Compare 2 new machine learning models, Balanced Random Forest Classifier and Easy Ensemble Classifier

We will then produce a report on the models evaluated to make a recommendation on the machine learning model that should be used to predict credi risk.

## Model Output / Results

### Naive Random Oversampling (D1)

Balanced Accuracy Score 62.9%

Confusion Matrix: 

![image](https://user-images.githubusercontent.com/91839403/159556169-ec07af29-c8a2-47dd-a9d5-cd11f7fd0a21.png)

Imbalanced classification Report

![image](https://user-images.githubusercontent.com/91839403/159556297-1829136c-9a33-4100-b0e2-a2716a4bf0c4.png)


### Random Oversample with SMOTE (D1)

Balanced Accuracy Score 62.0%

Confusion Matrix: 

![image](https://user-images.githubusercontent.com/91839403/159556597-5051a7af-37c9-4916-bd4c-1772fa1360e3.png)

Imbalanced classification Report

![image](https://user-images.githubusercontent.com/91839403/159556685-53220413-7ed6-490d-89da-36dad1c400e2.png)

### Undersampling with the ClusterCentroids algorithm (D1)

Balanced Accuracy Score 62.0%

Confusion Matrix: 

![image](https://user-images.githubusercontent.com/91839403/159557370-612d8267-236e-4700-bcfd-cdffdda1ddbf.png)

Imbalanced classification Report

![image](https://user-images.githubusercontent.com/91839403/159557441-f8c6f54e-8bea-4399-94bf-8cbd555c0f66.png)

### Over / Under sampling Combinatorial analysis with SMOTEENN (D2)

Balanced Accuracy Score 51.3%

Confusion Matrix: 

![image](https://user-images.githubusercontent.com/91839403/159558065-bba4c4af-a5d8-4a61-9071-71057a46e494.png)

Imbalanced classification Report

![image](https://user-images.githubusercontent.com/91839403/159558148-35776d40-d9f0-443d-98d0-11a679b24ee2.png)


## Balanced Random Forest Classifier (D3)

Balanced Accuracy Score 78.8%

Confusion Matrix: 

![image](https://user-images.githubusercontent.com/91839403/159559387-8005d121-21ad-4f27-9c88-4b179d1c7a14.png)


Imbalanced classification Report

![image](https://user-images.githubusercontent.com/91839403/159559582-19122c74-9278-4529-b7a4-c9c912ada6ab.png)

Feature Importance Ranking

![image](https://user-images.githubusercontent.com/91839403/159559906-8ef0c3e3-4e26-4125-8c6b-62843293f00f.png)


## Easy Ensemble AdaBoost Classifier (D3)

Balanced Accuracy Score 93.2%

Confusion Matrix: 

![image](https://user-images.githubusercontent.com/91839403/159560420-57daa7a6-0536-4488-a9a8-e21c77036e78.png)

Imbalanced classification Report

![image](https://user-images.githubusercontent.com/91839403/159560489-83392ebf-38a1-41c0-8d76-c05f2f479968.png)

## Conclusions and Recommendation

### Recommended Machine Learning Model: 
#### Easy Ensemble AdaBoost Classifier 
###### (See below for explanation)

The results shown below show that the Balanced Random Forest Classified and the Easy Ensemble AdaBoost Classifier have the highest balanced accuracy score wt 78.8% and 93.2% respectively.  The performance of the under and oversampling modles are well below these and are disqualified due to poor accuracy results.

With the highest accuracy score The Easy Ensemble Adaboost module could be a good choice, To evaluate further we looked at the High and Low risk performance and the associated f12 scores of these two models. Here the Easy ensemble modle shows a 9% precision vs 3% for the Balanced Random Forest classifier (and 1% for all others)  Clearly 9% is the worst performing here.  The Easy Ensemble AdaBoost Classifier also had a 92% sensitivity vs 70% for the Balanced Random Forest Classifier.  
Both models were similar on the low risk, we are focused on the high risk as that is where we want to make sure we dont make a mistake in lending or assessiing credit risk.  Finally the f1 scores were compared.  The Balanced Random Forest Classifier had an f1 of .93 vs the Easy Easy Ensemble Ada Boost classifier had an f1 score of .97.  There are differences to note in the performance of High risk and Low risk f1 scores for in the specific categories of performance.  These differences might be worth additional risk assessment and possible cost of error.  Overall the Easy Ensemble Model AdaBoost classifier had the highest accuracy and f1 score making it the recommended model for use in asssessing credit risk.


Summary Table of Model Results:

						
![image](https://user-images.githubusercontent.com/91839403/159567084-dc883421-4904-4a33-97fa-7407597ff672.png)
	
