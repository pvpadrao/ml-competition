# Machine Learning Competition
Final project submitted to FIU CAP5610 Introduction to Machine Learning (Spring/2022). 

In this project, we built an image classifier to classify fashion images into one of 4 categories: Apparel, Accessories, Personal Care, Footwear. The accuracy obtained was 99.49% and we ended up first place among other 9 groups

Group Members: Paulo Padrao, [Jose Fuentes](https://github.com/Xioeng), Prasanth Annam, Sergio Torres

## Data Description

``fiu-cap5610-spring22`` contains the following files:

* ``train.csv`` - the training set.
* ``test.csv`` - the test set
* ``sample_submission.csv`` - a sample submission file in the correct format
* ``images`` - folder containing all the train and test images

**Dateset Columns**

``img_id`` - id of the input images. The corresponding image file name is ``img_id.jpg``.

``label`` - label of the corresponding image

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
* We ended up first place among other 9 groups


