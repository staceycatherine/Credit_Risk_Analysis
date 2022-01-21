# Credit_Risk_Analysis
## Overview
Apply Machine Learning to Evaluate Credit Card Risk
After cleaning the data and splitting it into testing and training categories, we used the following algorithms to determine which one results in the best performance.

## Results shown in classification reports. 
* Oversampling with Naive random algorithm 
 ![image](https://user-images.githubusercontent.com/89313168/150556295-479c3378-5585-4042-b36b-03ae269af3a4.png)
    ##### Balanced Accuracy Score = 0.6473707152052903
    
 _____________________________________________________________________________________________________________________________________________________________________________

* Oversampling with SMOTE algorithm 
 ![image](https://user-images.githubusercontent.com/89313168/150556728-4ff72b15-12ce-48bd-8057-442fb06d9d75.png)
     ##### Balanced Accuracy Score = 0.6621602612787003
     
_______________________________________________________________________________________________________________________________________________________________________________

* Undersampling with ClusterCentroids resampler
 ![image](https://user-images.githubusercontent.com/89313168/150558221-c1e7517a-c7bf-4059-8f21-7d2fb47deb19.png)
    ##### Balanced Accuracy Score = 0.6621602612787003
    
_______________________________________________________________________________________________________________________________________________________________________________    

* Combination sampling with SMOTEEN
  ![image](https://user-images.githubusercontent.com/89313168/150560244-dd33c806-660a-417c-9e50-20b67228ae64.png)
     ##### Balanced Accuracy Score = 0.5442661782548694
     
_______________________________________________________________________________________________________________________________________________________________________________

* Ensemble algorithm using Balanced Random Forest Classifier
 ![image](https://user-images.githubusercontent.com/89313168/150560786-96bcfa31-9ca9-45e5-84bc-55f926501155.png)
   ##### Balanced Accuracy Score = 0.7885466545953005
   
______________________________________________________________________________________________________________________________________________________________________________
   
* Easy Ensemble Adaboost Classifier
 ![image](https://user-images.githubusercontent.com/89313168/150561237-f11afe2a-9025-40a3-b135-e8c88ef62db1.png)
    ##### Balanced Accuracy Score = 0.9316600714093861
    
_______________________________________________________________________________________________________________________________________________________________________________    
    
## Summary
We can see that the precision for all models is low for high risk and high for low risk. The balanced accuracy scores for the oversampling and undersampling are similar, 0.65-0.66 with a drop to 0.54 using SMOTEEN. Balanced Random Forest Classifier resulted in a higher balanced accuracy score of 0.79, and Easy Ensemble AdaBoost produced an even higher balanced accuracy score of 0.93. Following a similar pattern, the F1 scores for high risk using over and undersampling range from 0.01-0.0 with low risk showing a range of 0.57-0.75. The Ensemble algorithms provided higher F1 scores with both Random Forest and Easy Ensemble Adaboost yielding high risk 0.16, low risk 0.97. None of the models performed well with the given data set to predict the high risk applicants. I would not recommend using any of them to predict risk. 








