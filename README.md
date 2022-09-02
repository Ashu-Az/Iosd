# Iosd 

In this project , I implement a support vector machine (SVM) model to predict the hazardous objects which are close to the earth.


## Task 1 
Implement kernel SVM for classification and provide a comparative study using different kernels(linear, polynomial, gaussian, sigmoid, RBF etc) using precision and f1-scores. 

https://github.com/Ashu-Az/Iosd/blob/main/Iosd.ipynb

## Documentation
In the Task 1:
    1). After importing required dependies , I checked basic info about the dataset .

    2). Then i did analysis of the correlated data , I removed some unwanted columns to make the model more clear.

    3). After removing the unnecessary attributes , i used one hot encoding technique to divide the target value in two attributes to train the model.

    4). After preparing required dataset , I did stastical analysis and data visualization 

    5). Then i divided training and test datasets to train the model and implemented support vector machine (svm) kernels to do a comparative study between them

 * I implemented 4 types of different kernels i.e., linear , rbf , polynomial and sigmoid . In all of those kernels rbf have the best accuracy score

SVM finds optimal boundaries of the datapoints.

In this model i used support vector classifier as the method to draw the boundaries, SVC classify the datapoints who lie close to the hyperplane , whose distance is perpendicular to the hyperplane.

* linear kernel:

      In linear kernel i used gamma function as auto that means it will automatically take the relevant linear clasifier coefficient.
    then i scaled X_train and X_test as it would take a lot of time in training the model as the classifier.fit() takes lot of time for large datasets , I used scaling to normalize the data values for all datapoints to make them in range 0 to 1.
    In classifier variable i assigned the svm model to train the model using X_train and y_train.   
    Then to check the accuracy of the model i used X_test datavalues to predict the output value and assigned the prediction in y_predict.
    Then i used classification_report() method to check the efficiency of the model.
* rbf kernel , polynomial and sigmoid :
    I did the same process for rbf kernel too as , i just had to change the kernels name.








## Task 2
Try implementing a neural net for the above dataset as a binary classifier. You may use any AI library[*] like scikit, Tensorflow, pyTorch etc.

https://github.com/Ashu-Az/Iosd/blob/main/Iosd.ipynb

## Intuition
In Task 2 , I implemented aritificial neural networl using tensorflow and keras
* after implementing the neural network , i evaluated ANN efficiency using precision and recall

Artficial Neural Network:

    I made 3 layers neural network as , Input layer , Hidden layer and Output layer .

    In input layer i choosed 6 neurons as their are 6 attributes to start with.
    
    In hidden layer i added 3 neurons as i used 1/2 times the number of input neurons and in output layer i used 1 neuron as we have to predict only 0 and 1 , also in output layer i took activation as sigmoid as we have to predict only two outcomes.

    Then i evaluated the ANN using model.evaluate() method. 

     
