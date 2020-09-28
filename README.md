# Machine Learning (Predicting Credit risk)

## Credit Risk
Credit risk is an inherently unbalanced classification problem, as the number of good loans easily outnumber the number of risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes.

## Native Oversampling
First we compared two oversampling algorithms to determine which algorithm results in the best performance. We oversampled the data using the native random oversampling algorithm and the SMOTE algorithm.

When utilizing random oversampling, the precision for finding low-risk loan applicants is 100% but high risk is 1%. The recall is better for detecting high-risk applicants at 51% while the recall rate for low-risk applicants is 63%.

## Smote
Algorithm predicted a little bit better than naive random pversampling, however, the F1 score is not robust enough for this model to be span into a full commercial application.

## Undersampling
The F1 score for low-risk applicants is 0.80 and 0.02 for low and high-risk applicants, respectively. This means the model is better at predicting low-risk applicants but not very good at detecting high-risk applicants, resulting in loans potentially being given out to high-risk applicants.

The balanced accuracy score for this model is 58%.

## Combination Sampling
We finally tested a combination over- and under-sampling algorithm to determine if the algorithm results in the best performance compared to the other sampling algorithms above. We resampled the data using the SMOTEENN algorithm.

## Recommendation 
AdaBoost model shows the most reliable results and can likely be used in commercial application with some additional testing.
