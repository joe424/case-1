# Digital_medicine_case1

Case presentation 1: Smoking Status Detection 
## Environment
google colab
## Implementation approach
### pattern_matching.ipynb
Function: Recognize patterns using regx.
* parse_file():<br>Take training and testing data as input. 
Output train_form.csv / test_form.csv with predicted label(type), which will be later used and trained in main.ipynb.
* judge_output():<br>Output the accuracy achieved by regx method 


### [main.ipynb](joe424/digital_medicine_case1/blob/master/main.ipynb) 
Function: Train data and output the predict label.
* Taking <font color=#336699>train_form.csv</font>, <font color=#336699>test_form.csv</font> as input, and then train the data sets using PyTorch provided Model, so called "glove.6B.100d", which is featured in text pattern.
* Hyper parameters
>         embedding_dim = 100
>         hidden_nodes = 32
>         num_layers = 2
>         output_nodes = 4
>         dropout = 0.2
>         batch sizes = 8
>         epochs = 200
### output

N row of predicted label representing N test data respectively, given that
>  0 : "current_smoker", 1 : "non_smoker", 2 : "past_smoker", 3 : "unknown"
