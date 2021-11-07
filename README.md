# Module19-Challenge:Neural_Network_Charity_Analysis

## Overview of the analysis:
This project is designed to create a binary classifier ,by machine learning and neural networks, that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.


## Results:
### Data Preprocessing:
 - What variable(s) are considered the target(s) for your model?  
   The variable "IS_SUCCESSFUL" is the target for the model.
   
 - What variable(s) are considered to be the features for your model?  
   The variables including "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS" and "ASK_AMT" are considered to be the features.
   
 - What variable(s) are neither targets nor features, and should be removed from the input data?  
   The variables "EIN" and "NAME" should be removed from the input data.
 
 ### Compiling, Training, and Evaluating the Model
 - How many neurons, layers, and activation functions did you select for your neural network model, and why?  
   The initial model included two layers that the first layer had 80 neurons and the second one had 30 neurons. The numbers of neurons and layers depended on the size of input data which was 5 rows and 41 columns.
   
 - Were you able to achieve the target model performance?  
   The original model cannot achieve the performance with 75% accuracy, which is only 69.56%.
 - What steps did you take to try and increase model performance?  
   (1) Attempt 1 model: Add more data into bin 'Other' from variable "APPLICATION_TYPE". The updated accuracy is :67.94%.  
   (2) Attempt 2 model: Remove two variables "SPECIAL_CONSIDERATIONS" and "STATUS" from input data.The updated accuracy is :53.33%.  
   (3) Attempt 3 model: Add more layers and neurons to model.The updated accuracy is :44.54%.  
### Summary
After three attempts, these models were unable to create a model that could preform a 75% accuracy rating. There were several possible methods to improve the model:  
 (1) There were too many columns. The next attempt can be consided to reduce the size of input data by removing or combining the variables with high covariance.
 (2) The activation functions were not suitable for each layers. The following attempt can be consider to fit other activation functions.
 (3) Check other pairs of layers and neurons to refit model.
 (4) Check the outlier of input data.
