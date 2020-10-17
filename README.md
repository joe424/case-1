# Digital_medicine_case1

Case presentation 1: Smoking Status Detection 

## Implementation approach
### pattern_matching.ipynb
Function: Recognize patterns using regx.
Take training and testing data as input, and output train_form.csv, test_form.csv. After inputing training data ,they will get the predicted label(type) first, which will be later used and trained in main.ipynb.

### main.ipynb 
Function: Training data and output the predict label
Taking the output of parse.ipynb as input,and then train the data sets using PyTorch provided Model ,so called "glove.6B.100d", which is featured in text pattern.

### output

N rows of predicted labels representing N test data respectively, given that
>  0 : "current_smoker", 1 : "non_smoker", 2 : "past_smoker", 3 : "unknown"

### details
https://docs.google.com/document/d/1rMlVUad5CVz59byDkLrGY3FJckvJttZtNLYZUJGg5Fw/edit?usp=sharing






		













