******Notice: ****** -- 
1. We git cloned our GitHub repository at the first code cell to load data files, which contains the whole train, dev and test files. 
2. We made some modification on train(), which will return prediction output by given the test dataset we found online.


******How to run:****** -- 
Directly compile all the code.


******Parameter setting***** -- 
The parameters have been defined in the Config class. 
There is an instance(names as “config”) of Config that have been created. 
We computed our hyper-parameter test by modifying the parameter in Config & “epochs”. 
The parameters can be modified as below.

For example,
“config.pre_trained = True”       (“Ture” - Approach 1 with pre-trained  Approach 2 with no pre-trained)
“config.lr = 0.1”                       (Learning rate = 0.1)
“config.dropout = 0.1”              (Dropout rate = 0.1)


******For the Approach 1****** -- 
Run all cells before and including the cell of Approach ONE. 
“config.pre_trained” have been set to True, and the best parameters we found have been set. 
Apart from the output of train and validation, we also add the test output of each epoch.


******For the Approach 2******
After computing approach 1, run the last cell: Approach TWO. 
“config.pre_trained” have been set to False, other parameters may setted to perform the best performance. 


******Generate CSV output****** -- 
We made some small modification to train() function. 
It will return the predication of the test case of the competition, 
So the last section will be used to generate the CSV output file, which named”task-1-output.csv”


 *****Example code of our hyperparameter tuning ******* -- 
We leave some example code for how we run our hyperparamter tuning and how we draw the analysis diagram, it been placed at the bottom of our notebook.
Meanwhile, if you would like to run our hyper-parameter experiments, you also need to delete the result part of the train() and replace it with the one we made comments.


