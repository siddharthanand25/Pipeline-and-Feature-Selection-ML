# Pipeline-and-Feature-Selection-ML

## Pipelines Objective
To use a Pipeline to repeat evaluation of the previous assignment done using Hold-Out testing. In the Algorithm Bias Assessment the results were coming out to be unstable with different train-test split, that's why this time we will be utilizing Cross-Validation technique with the Pipeline strategy to point out the diffeneces in both the strategies.
To start with, load the hold-out evaluation strategy from the first assignment
Evaluate this strategy with the cross-Validation using Pipeline
Point out the results obtained by above two techniques.

## Objective: To assess the impact of feature selection on Training and Test dataset

Utilizing Information Gain Theory for the feature selection to determine the relevance of attribute in the Heart Data set

Utilizing sequential feature selection to automatically select subset of the feature that are more relevant to the given problem statement
Our main aim is to reduce the computational cost invloved as well as remove the unnecessary features. This will be helpful in removing errors.
Sequential feauture selection is a wrapper approach that performs addition or removal of attributes based on the performance of the classifier. This process happens until we reach to our desired number of features.
INPUT: the input will be all the attributes of the dataset Provided
OUTPUT: We will have to provide the number of feautures in advance, then the output will be subset of the features provided.In our computation, I'll be providing K_features=8


## Outcomes of the methods: Forward Sequential Search and Backward Elimination
Accuracy obtained from Forward search approach comes out to be 79%
Accuracy obtained from Backward elimination approach comes out to be 85%. Hence, we will be going forward with this method.
Sequenctial forward search and backward elimination have been performed on Heart training dataset and evaluated its efficiency on Heart testing data set

## Outcomes from the performance metrics => F1Score, Precision Value, Recall and Accuracy Score¶
The Accuracy and the precision value of the classification model is decent enough, with 85 and 80 percent.
The Recall value is low in comparison to other metrics. But since this classificaiton model is of medical diagnosis, Hence the true positive rate is significantly important. It is the value associated with "the total no. of data predicted postive correctly to the total no. of data that are in class positve." It is helpful in the scenarios where our system is predicting the class label as death event and it is actually a death event.
For increasing the performance of the recall, we are considering SMOTE technique to Upsample the training Hearth dataset.

## Final Outcome
After applying the SMOTE Technique on the Hearth Training data we have identified that The Effects on Evaluation metrics are:
The Accuracy and Recall scores have significant postive effects. The Accuracy rose from 85 to 87% and Recall value rose from 72 to 81
The precision value has little or no effect on Upsampling
