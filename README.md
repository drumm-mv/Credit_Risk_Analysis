# Credit_Risk_Analysis
Using knowledge of the imbalanced-learn and scikit-learn libraries, evaluate three machine learning models by using resampling to determine which is better at predicting credit risk.

## Overview of the analysis:
Employ different techniques to train and evaluate models with unbalanced classes. Use the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Oversample a credit card credit dataset using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. And finally compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results:
### RandomOverSampler algorithm

    Confusion Matrix
    
<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Predicted 0</th>
      <th>Predicted 1</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Actual 0</th>
      <td>72</td>
      <td>29</td>
    </tr>
    <tr>
      <th>Actual 1</th>
      <td>6812</td>
      <td>10292</td>
    </tr>
  </tbody>
</table>
</div>


    Accuracy Score : 0.6573009382322703
    Classification Report
                       pre       rec       spe        f1       geo       iba       sup
    
      high_risk       0.01      0.71      0.60      0.02      0.65      0.43       101
       low_risk       1.00      0.60      0.71      0.75      0.65      0.42     17104
    
    avg / total       0.99      0.60      0.71      0.75      0.65      0.42     17205
    
    

### SMOTE algorithm

    Confusion Matrix
    
<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Predicted 0</th>
      <th>Predicted 1</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Actual 0</th>
      <td>64</td>
      <td>37</td>
    </tr>
    <tr>
      <th>Actual 1</th>
      <td>5288</td>
      <td>11816</td>
    </tr>
  </tbody>
</table>
</div>


    Accuracy Score : 0.6622479600626106
    Classification Report
                       pre       rec       spe        f1       geo       iba       sup
    
      high_risk       0.01      0.63      0.69      0.02      0.66      0.44       101
       low_risk       1.00      0.69      0.63      0.82      0.66      0.44     17104
    
    avg / total       0.99      0.69      0.63      0.81      0.66      0.44     17205
    
    


### ClusterCentroids algorithm

    Confusion Matrix
    
<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Predicted 0</th>
      <th>Predicted 1</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Actual 0</th>
      <td>70</td>
      <td>31</td>
    </tr>
    <tr>
      <th>Actual 1</th>
      <td>10324</td>
      <td>6780</td>
    </tr>
  </tbody>
</table>
</div>


    Accuracy Score : 0.5447339051023905
    Classification Report
                       pre       rec       spe        f1       geo       iba       sup
    
      high_risk       0.01      0.69      0.40      0.01      0.52      0.28       101
       low_risk       1.00      0.40      0.69      0.57      0.52      0.27     17104
    
    avg / total       0.99      0.40      0.69      0.56      0.52      0.27     17205
    
    


### SMOTEENN algorithm

    Confusion Matrix
    
<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Predicted 0</th>
      <th>Predicted 1</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Actual 0</th>
      <td>81</td>
      <td>20</td>
    </tr>
    <tr>
      <th>Actual 1</th>
      <td>7298</td>
      <td>9806</td>
    </tr>
  </tbody>
</table>
</div>


    Accuracy Score : 0.6876481906843631
    Classification Report
                       pre       rec       spe        f1       geo       iba       sup
    
      high_risk       0.01      0.80      0.57      0.02      0.68      0.47       101
       low_risk       1.00      0.57      0.80      0.73      0.68      0.45     17104
    
    avg / total       0.99      0.57      0.80      0.72      0.68      0.45     17205
    
    


### BalancedRandomForestClassifier algorithm

    Confusion Matrix
    
<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Predicted 0</th>
      <th>Predicted 1</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Actual 0</th>
      <td>71</td>
      <td>30</td>
    </tr>
    <tr>
      <th>Actual 1</th>
      <td>2153</td>
      <td>14951</td>
    </tr>
  </tbody>
</table>
</div>


    Accuracy Score : 0.7885466545953005
    Classification Report
                       pre       rec       spe        f1       geo       iba       sup
    
      high_risk       0.03      0.70      0.87      0.06      0.78      0.60       101
       low_risk       1.00      0.87      0.70      0.93      0.78      0.62     17104
    
    avg / total       0.99      0.87      0.70      0.93      0.78      0.62     17205
    
    


### EasyEnsembleClassifier algorithm

    Confusion Matrix
    
<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Predicted 0</th>
      <th>Predicted 1</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Actual 0</th>
      <td>93</td>
      <td>8</td>
    </tr>
    <tr>
      <th>Actual 1</th>
      <td>983</td>
      <td>16121</td>
    </tr>
  </tbody>
</table>
</div>


    Accuracy Score : 0.9316600714093861
    Classification Report
                       pre       rec       spe        f1       geo       iba       sup
    
      high_risk       0.09      0.92      0.94      0.16      0.93      0.87       101
       low_risk       1.00      0.94      0.92      0.97      0.93      0.87     17104
    
    avg / total       0.99      0.94      0.92      0.97      0.93      0.87     17205
    
    


## Summary:

Out of the first four Over/Under sampler algorithms RandomOverSampler, SMOTE, ClusterCentroids, and SMOTEENN, the SMOTEENN algorithm had the best balanced accuracy score at 68.8% and the SMOTE oversampler had the best recall score at 69%

From testing the BalancedRandomForestClassifier and EasyEnsembleClassifier algorithms, the easy ensemble classifier algorithm works best for this data set. The easy ensemble classifier had the best balanced accuracy score at 93% and the best recall score at 94%
