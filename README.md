# Neural_Network_Charity_Analysis

## Overview
The request is to help a charity foundation's staff member create a predictive model that determines which applicants will be successful if funded by the foundation.  

## Results
* What is considered the target for the model? 
    - Correct prediction of success rate as defined in column Is_Successful
    
* What are considered to be the features for the model?
     - Application Type
     - Income Amount
     - Special Considerations
     
* What variables in the data are not features or targets and should be removed? 
     - Name
     - Employer Identification Number
     An argument can also be made to remove the following: 
     - Use Case
     - Affiliation
     - Ask Amount
     
* How many neurons, layers, and activation functions were selected for the neural network model, and why?
    - Initially, two layers with a spread of 80/30 neurons were chosen for the model.
    
* Was target model performance achieved?
    - Target model performance of 75% was not achieved and the initial model came closest at 68.5%
    
* What steps were taken to try and increase model performance?
    - First optimization attempt decreased the neurons in the first layer and increased the neurons in the second layer. This 70/40 split resulted in 62.8% accuracy.
    - Second optimization attempt increased both layers slightly. This 75/60 split resulted in 64.1% accuracy.
    - Third optimization attempt increased the first layer, decreased the second, and added a third layer. This 80/50/20 split resulted in 53.6% accuracy.

## Summary
While this model can inevitably be efficient by testing multiple changes to the model, I believe the model would be better served by initiating a Balanced Random Forest Classifier model to see which features are highly weighted for involvement in the predictive model, dropping the lower-rated fields, and then continuing with the neural network model. 
