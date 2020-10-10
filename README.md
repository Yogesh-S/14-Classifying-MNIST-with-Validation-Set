# 14-Classifying-MNIST-with-Validation-Set

In this notebook, we use two different approaches to predict hand written digits using Pytorch.  
> * Training Model without Validation Data  
> * Training Model with Validation Data  

There are few advantages of using Validation Dataset while training Neural nets,  
 > * Avoid Overfitting - Validation data will accompany in tuning the hyperparameter (no. of epochs) required to train the model. Validation dataset will basically help us know where to stop the model training as shown in figure below.
 
![alt text](https://github.com/Yogesh-S/14-Classifying-MNIST-with-Validation-Set/blob/main/Overfitting.JPG?raw=true)

> * Choosing between multiple NN architecures

# Why can't we use test set as validation set?

Even though the model doesn't use the validation sets for updating weights, our model selection process is based on how the model performs on the both training & validation sets.
So, in the end, the model is based in favor of the validation set.

  Thus, we need a separate test set of data to truly see how our seleted model generalizes and performs when given data it really has not seen before.

<br/><br/>

  


Note: Since MNIST is basic dataset, there is not much difference in the Prediction accuracy on test data with/without validation.
