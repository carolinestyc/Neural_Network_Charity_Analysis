# Neural_Network_Charity_Analysis
  Challenge 19
  
## Project Overview

During the course of this project, I was creating a machine learning model to predict if applicants who receive Alphabet Soup Co. funding will be successful. Successful is defined by classification into TRUE or FALSE. Alphabet Soup Co. wants to provide funding to everyone but they understand not all companies will be succesful. This model will help them figure out if their funding to the company will lead to successful outcomes so they don't fund companies that aren't going to succeed. 

Using data manipulation, creating training and testing sets, and analyzing the models, a neural network is created. The results are explored below.

## Resources
            Data Source: charity_data.csv

            Software: Jupyter Notebook
            
## Results

* Data Processing
  * ID columns "EIN" and "NAME" are removed from the model because they are not target or feature variables.
  * IS_SUCESSFUL is the target variable for the model.
  * APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT are the feature variables for the model.

2 Hidden Layers
80 neurons (Layer1), 30 neurons(Layer2)
Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classifcation problems as this and relu is for nonlinear datasets.
Removed "USE_CASE_Other","AFFILIATION_Other" columns.

## Attempt #1
* Compiling, Training, and Evaluating the Model
  * 2 hiden layers: (100) neurons in Layer 1 and (30) neurons in Layer 2. Used relu activation functions for the hidden layers and sigmoid for the output because it is best for classification problems.
  * Accuracy is 73.06%: did not achieve target model performance.
  * I added more neurons to try and increase model performance.

<img width="609" alt="Attempt1" src="https://user-images.githubusercontent.com/96352625/168411212-4a204697-fefc-4fab-b3ce-0701ed552abd.png">

## Attempt #2
* Compiling, Training, and Evaluating the Model
  * 3 hiden layers: (80) neurons in Layer 1, (35) neurons in Layer 2, (10) neurons in Layer 3. Used relu activation functions for the hidden layers and sigmoid for the output because it is best for classification problems.
  * Accuracy is 72.85%: did not achieve target model performance.
  * I added more hidden layers and used fewer neurons but the accuracy went down.
 
<img width="605" alt="Attempt2" src="https://user-images.githubusercontent.com/96352625/168411217-e996439a-0a3d-4890-9974-efa6ed33e428.png">

## Attempt #3
* Compiling, Training, and Evaluating the Model
  * 3 hiden layers: (80) neurons in Layer 1, (30) neurons in Layer 2, (15) neurons in Layer 3. Used relu activation function for the first hidden layer and sigmoid for the 2nd, 3rd, and output to add more classification. 
  * Accuracy is 73.02%: did not achieve target model performance.
  * I change the activation functions and altered the number of neurons but the target was not met.
 
<img width="609" alt="Attempt3" src="https://user-images.githubusercontent.com/96352625/168411222-c1dfa3bf-f0e2-4f8f-a7d8-e819f6206d3f.png">

# Summary
To achieve a higher accuracy I tried changing the number of neurons, the activation functions, and the number of layers but I was not able to get above 73%. Just 2% short of the goal. There may be features not included in the data set that need to be included in the analysis to achieve over 75%.
