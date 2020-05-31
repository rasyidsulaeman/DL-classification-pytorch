# FashionMNIST datasets

This notebook shows how to train a simple CNN using pytorch library.

MNIST dataset usually was used to check and evaluate whether our built model has been correct and reached some desired accuracy. Yet, MNIST dataset is too simple because they show a simple patten, although they have slightly different picture for describing number "2" for example, this picture still share the same pattern thus it's not surprising to achieved 80 even 90 % accuracy. 

On the other hand, relative to MNIST dataset FashionMNIST dataset has a little bit complexity in their image. Fashion dataset contains 10 classes, each of which decribes fashion product. You can check for more detail of the this dataset on [FashionMNIST](https://github.com/zalandoresearch/fashion-mnist).

## Convolution Neural Network Architechture

The common CNN architechture is depicted in the below figure. 

The concepts is as follow:

1. Input images is convolved by certain kerner/filter/features detector and get features map. 
2. The convolutional operation run in linear order, therefore we should use the relu function. It breaks up the linearity.
2. Pooling take the unique value in the features map. Maxpooling means that it takes the maximum value within certain kernel size. This is important since it reduces the size of input images along with preserves the unique features.
3. Before flowing into the fully-connnected layer, they should be flattening
4. Fully-connected layer

![CNN](cnn.png)
