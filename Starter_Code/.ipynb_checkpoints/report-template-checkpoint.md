# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis. - 

The company is a platform that provides peer-to-peer lending services, connecting individual lenders and borrowers while providing a credit risk analysis service.
However, it faces the problem that the credit risk classification is imbalanced because healthy loans outnumber risky loans.

* Explain what financial information the data was on, and what you needed to predict. - 

The data presented was over 77,500 credit scores that summarized such data points as loan size, interest rate, borrower income, debt to income ratio, number of accounts and derogatory marks. Using a logistics regression model I needed to understand the accuracy of the imbalanced data, then fit the data and proceed to predict the accuracy of said data. 

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
As per the value counts function, there are 75,036 data points considered as 0 or healthy loans and there are 2,500 data points considered as 1 or high-risk loans. 

* Describe the stages of the machine learning process you went through as part of this analysis.
There were two main stages: first I created a logistics regression model using the original data, fitting the model and seeking predictions from said data. Second, I created and oversample set of data that had a balanced set of data, i.e. the set labels had an equal number of data points. Then, as in the first stage, I fitted the model and sought a prediction.  

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
As described above, the method used was with the functions of Logistics Regression, oversample data for the resampling and model predictors.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
The 1st model indicates that of 18,765 credit samples, the model predicted correctly 18,663 as healthy loans whereas 102 loans were incorrectly predicted as healthy. Also, of the 619 credit samples, the model predicted correctly 563 as high-risk loans whereas 56 loans were incorrectly predicted as high-risk.
The accuracy, precision and recall scores are respectively, 0.95, 0.99 and 0.99


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
The 2nd model indicates that of 18,765 credit samples, the model predicted correctly 18,649 as healthy loans whereas 116 loans were incorrectly predicted as healthy. Also, of the 619 credit samples, the model predicted correctly 615 as high-risk loans whereas 4 loans were incorrectly predicted as high-risk.
The accuracy, precision and recall scores are respectively, 0.99, 0.99 and 0.99  
  

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
The oversample model seems to perform best mainly because of the higher accuracy level that it shows than the original imbalanced data.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
No, I believe the problem here is the undersampling of the data as the high-risk loans are underrepresented. The model 2 allows for a correction in this deficiency in the data.

Overall, I would recommend using the model 2 with oversample data because it shows a higher level of accuracy.

If you do not recommend any of the models, please justify your reasoning.
