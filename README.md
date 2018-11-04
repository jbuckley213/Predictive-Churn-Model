# Predictive-Churn-Model

Overview
=========
This project is to predict if a customer will leave the bank using an artifical neural network. 

Dependencies
=========
* Numpy (http://www.numpy.org/)
* Pandas ```pip3 install pandas```
* Keras ```pip3 install keras```

Neural Network
=========
The neural network has 11 inputs nodes. The nodes are multiplied by weights and a bias added to map to the output. Random weights are given to the input nodes to begin and are updated through backpropagtions. The weights are changed by how much the intial prediction was incorrect, in this case the binary cross entropy loss function is used. The model is trained on 80% of the data and tested on 20% of the data to test the model is not overfitting. 

Results
========
The neural network trained for 100 epochs for 8000 steps per epoch. The accuracy of the training data is 0.8337 with a loss of 0.402. The validation accuracy is 0.842 and the validation loss is 0.398. The accuracy score is satisfactory but the loss is a concern.
From the confusion matrix it can be seen that there a 277 false negitives and only 128 true negitives. The problem may stem from insufficient data as nearly 80% of the data has an output 0. A larger and more diverse data set would help the models preformance.

Acknowledgments
========
This project was completed with the help of Udemys Deep Learning course
