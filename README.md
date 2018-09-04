# Neural Network exercise
This repository have the data and the code used to create a neural network to predict the slope and intercept.

The prediction on the tast data can be found in the file 'submission.csv'.

To run the neural network ('lr_inter.ipynb' file), all the libraries in the first cell must be installed.

The neural network use 10 points in the x-axis and their corresponding in the y-axis along with slope and intercept for this set of points to learn the best way to do a regression. In the training data we can see 100,000 rows with those 10 set of points used to train the network. 
Therefore, to use this neural network to predict the slope and intercept in any data, we need to enter 10 set of points (x and y pairs) and the predicted slope and intercept can be saved in a csv file as shown in the last cell of the notebook.



I created a neural network with three layers. The first one is the input layer with 45 neurons. Lower numbers were tested but the results were not good. The second, or hidden layer, have 30 neurons. I also tested other activation functions but relu for the first and second layer showed best results (lower mse and mae). Last layer give us two outputs (slope and intercept) and use linear as the activation function.
Other options like batch_size value were tested but I coudn't use numbers lower than the default value as batch_size number because of hardware limitations. I could have used google colab but when I tried to import the data to their notebook I received an error, then I used Jupyter Notebook in my own computer.


