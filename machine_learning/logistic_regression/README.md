# Module 12 Summary Report

## Overview of the Analysis

The purpose of this analysis is to determine whether a given loan is likely to default or successfully be repaid.  
  
The data used includes 77,536 loans, each with the following data:
  * Loan size  
  * Interest rate  
  * Borrower income  
  * Debt to income ratio  
  * Number of accounts  
  * Derogatory marks  
  * Total debt  
  
Of those 77,536 total loans, 2500 (3.2%) are defaults.  Because of this imbalanced dataset the analysis is done twice in order to highlight the technique of random oversampling, which resamples enough of the original instances to make the size of the smaller class equal to the size of the larger class. The analysis will make use of logistic regression as our classifier algorithm.  


## Results  
  
* Analysis 1 - original imbalanced dataset:  
  __Accuracy__: 95.2   
  __Precision__  
    * healthy loans: 1.00  
    * high-risk loans: 0.85  
    
  __Recall__  
    * healthy loans: 0.99  
    * high-risk loans: 0.91  

* Analysis 2 - rebalanced dataset:  
  **Accuracy**: 99.3  
  **Precision**  
    * healthy loans: 1.00  
    * high-risk loans: 0.84  
    
  **Recall**  
    * healthy loans: 0.99  
    * high-risk loans: 0.99  

## Summary  
  
Overall, we can see that both models produce relatively high accuracy. The precision for the high-risk loans is in both cases less than the healthy loans, and that precision remains the nearly the same regardless of rebalancing. Meaning they had a tendency to predict that more high-risk loans were healthy than was actually the case. The recall score did see significant improvement after rebalancing, moving from 0.91 to 0.99 for the high-risk loans. Meaning in this case that the model improved its ability to correctly predict high-risk loans. 
  
If we had to choose, it's more important to identify the high-risk loans than healthy ones. The loss of a potentially healthy loan that gets misclassified as risky is just an opportunity cost. A high-risk loan that gets misclassified as healthy is an actual loss.  In which case, the rebalanced data set gives us a better prediction for high-risk loans. We'll sacrifice a little bit of precision to get better recall.
