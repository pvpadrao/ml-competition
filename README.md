# Machine Learning Competition
Final project for FIU CAP5610 Introduction to Machine Learning (Spring/2022). 

In this project, we built an image classifier to classify fashion images into one of 4 categories: Apparel, Accessories, Personal Care, Footwear. 

## Model Details

### CNN Architecture
We used the DenseNet201 Architecture available in Tensorflow.

### Classifier Architecture
We used a fully connected neural network with:
* 256 Dense layer, ReLu activation
* Dropout layer p=0.3
* 128 Dense layer, ReLu activation
* Dropout layer p=0.3
* 128 Dense layer, ReLu activation
* Dropout layer p=0.3 
* 4 Dense layer, Softmax activation

## Simulation Details
* Compilation: categorical cross entropy, SGD optimizer with batch size of 32, 100 epochs, and learning rate of 0.01.
* The weights for the CNN were initialized using the ImageNet pre-trained weights. 
* The fully connected part was initialized randomly.
* This model has 18+ million parameters.

## Result 
* The accuracy obtained was 99.49%
* We ended up first place among other 7 groups


