# Credit_Risk_Analysis
## Overview
The purpose of my Machine Learning analysis was to run multiple types of tests to try and find the best one to predict which loans were bad and thus high credit risk, vs good loans and low credit risk. I did this by running a plethora of models and then scoring each of them using accuracy scores, along with confusion matrices, and finally classification reports to summarize and conclude my findings as shown below.

## Results
  - Naive Random Over Sampler model
    - Accuracy Score: 63%- which isn't ideal because there aren't that many high risk loans, so only catching 63% isn't good enough.
    - Precision: 1%- also not ideal especially coupled with a low recall rate below.
    - Recall: 59%- this means that this model only catches high risks a little over half the time which isn't a good business model.
<img width="728" alt="Screen Shot 2021-11-11 at 1 49 03 PM" src="https://user-images.githubusercontent.com/86524863/141352598-4ede3428-5cd6-413a-a444-95e3d0d03a9f.png">

 - SMOTE model
   - Accuracy Score: 64%- only catching 64% is not ideal when only dealing with a small number of high risk loans.
   - Precision: 1%- definitely too low when mixed with a low recall rate below.
   - Recall: 59%- the SMOTE model only catches high risk loans a little over half the time.
<img width="728" alt="Screen Shot 2021-11-11 at 1 53 01 PM" src="https://user-images.githubusercontent.com/86524863/141353013-ef60f4ae-af87-4856-9855-5e61bd22e7d1.png">

 - Cluster Centroids model
   - Accuracy Score: 67%- although we are increasing in accuracy score it's still not high enough for a good business model.
   - Precision: 1%- very low for a model especially combined with the other low scores.
   - Recall: 76%- this has taken a larger jump up compared to previous models, but still not satisfactory.
 <img width="709" alt="Screen Shot 2021-11-11 at 1 57 15 PM" src="https://user-images.githubusercontent.com/86524863/141353451-7f7a1b26-3861-406d-8e33-b71a98a552e6.png">

 - SMOTEEN model
   - Accuracy Score: 62%- This is back to being as low as our first 2 models- not good enough for a business.
   - Precision: 1%- not a good precision model score.
   - Recall: 70%- this has dropped from our Cluster Centroids model back down to worse levels- unsatisfactory.
 <img width="727" alt="Screen Shot 2021-11-11 at 2 00 45 PM" src="https://user-images.githubusercontent.com/86524863/141353831-049ce9cf-ef6f-4735-8634-8f6ec7249c86.png">

 - Balanced Random Forest Classifier model
   - Accuracy Score: 79%- this is our highest accuracy yet- definitely getting close to being satisfactory.
   - Precision: 3%- this triples our other 4 models precision score, which is great but there are more low risk loans compared to high risk loans.
   - Recall: 70%- we are at the same percentage as our SMOTEEN model, but the other scores are higher which helps the overall performance of this model.
<img width="726" alt="Screen Shot 2021-11-11 at 2 07 07 PM" src="https://user-images.githubusercontent.com/86524863/141354725-61bcb094-7e3f-47e1-a2fd-5b435cd52481.png">

 - Easy Ensemble AdaBoost Classifier
   - Accuracy Score: 93%- this is the highest score yet- and satisfactory for a business to make their decisions based off of. 
   - Precision: 9%- this tripled our last models precision and is the best score yet for precision.
   - Recall: 92%- this is fantastic because high risk loans are rare, but this will easily identify them to make informed decisions that save the company money.
<img width="722" alt="Screen Shot 2021-11-11 at 2 12 08 PM" src="https://user-images.githubusercontent.com/86524863/141355273-4d916f54-4345-49cc-b6dd-9393ee5daddf.png">

## Summary
In conclusion, the models that oversampled were unsatisfactory in their scores- which means they would have a hard time catching high risk bad credit loans. The same goes for the models that undersampled, both of these would not be good to use in a business model when trying to predict which loans to approve or deny. The Ensemble Classifier model gave us our best accuracy, precision, and recall percentage scores and would be the best option moving forward to use in a business setting. I would like to see this model used on more datasets before making a final decision, but the recall rate alone being at 92% along with an accuracy score of 93% would give the client what they're looking for. Start there and add more data more data more data to keep testing- happy credit approving!

