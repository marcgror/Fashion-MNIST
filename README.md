# Fashion-MNIST
One evolution of the MNIST dataset is the Fashion-MNIST, where the handwritten digits have been replaced by fashion items. It also has 10 classes, but as they are more diverse, the problem turns out to be more challenging than MNIST.

In this case, I implement an hyperparameter optimization framework (Optuna) to tune the hyperparameters of a Convolutional Neural Network (CNN). 

I wanted to try a different tool for hyperparameter optimization, Optuna, in contrast to Hyperopt, which I used with the MNIST dataset, looking for differences in performance, and more important, in the results obtained.

Hyperparameter tuning is one of the most important steps when training Neural Networks or ML algorithms, as it may incredibly improve the performance of the model.
## Data
The Fashion-MNIST dataset is loaded easyly from keras.datasets, then prepocessed as usual with the image classification tasks, and then fed to the CNN.
## Hyperparameter tuning
I chose to optimize:
  - the optimizer: from 'Adam' to 'SGD', the learning rate and the momentum(only for 'SGD')
  - number of Conv2D laters, with their respective units
  - the dropout rate for the Dropout layers
  
 ## Results
 After tuning the hyperparameters, the model scores 0.87 on the test set.
  
