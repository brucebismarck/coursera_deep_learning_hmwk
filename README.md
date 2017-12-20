# coursera_deep_learning_hmwk

## Course 1
#### Neural Network and Deep Learning. They are based on numpy. 
#### hmwk 1-5 belong to coursera deep learning specialization course 1
* hmwk 1 (optional) is used to let student have some basic understanding on numpy.
  - build sigmoid fuction / gradient of sigmoid
  - reshape(np.reshape), vector normalization (np.linalg.norm)
  - boardcasting and softmax
  - L1 L2 norm
  
* hmwk2 built a logistic regression on a 209 (m) * 64*64*3 image data set 
  - initialization (zeros init because of logistic reg)
  - basic forward and backward prop
  - Gradient descent
  - structure/shape of the feeding data. Each col contains a pic,rather than row.
  - Viz of cost changing
  
- hmwk3 buit a **shallow neural net** to do binary classification.
  - Two layers
  - Loop, forward/ backward chain, parameter update function
  - Hidden layer number of unit tunning.
- hmwk4 & hmwk5 buit a **'deep' neural net** to cat/non-cat calssification.
  - automatically do loop, forward, backward, cache of A_prev, W, b, grads, parameter update. (based on number of layers)
  - relu vs. sigmoid
  - homework 5 compared performance between two layers and 5 layers NN.
  
## Course 2 
#### Improving Deep Neural Net Hyper parameter tuning, regularization and optimization
#### hmwk 6-? belong to coursera deep learning specialization course 1
* hmwk6 implemented zero, random, he's initialization methods.  Kaiming He's method shows awesome output

* hmwk7 implemented L2 normalization and dropout methods. The backward prop with dropout has some tricky parts. You need to save the D2 amd D1 for A2 and A1 which did dropout, and apply D2 D1 to dA1 and dA2.

* hmwk8 implemented gradient check which is meaningless in pytorch LOL. But it still a good practice

* hmwk9 implemented gradient descent, momentem and Adam optimization algorithms in numpy. This might be the last one pynb file mainly completed with numpy

* hmwk10 Tensorflow Tutorial

## Course 3. Structuring Machine Learning Projects
No coding homeworks

## Course 4 CNN
* Week1 
  - Homework 1. Implement CONV, PADDING, POOL and forward prop in Numpy.
  - Homework 2. Apply simple Neural Net on SIGNS (finger numbers) dataset, which used in prev DNN model.
            With CNN, we can train the model to tell thumb up as 1.
            
* Week2 
  - Homework1.  Keras Tutorial 
  - Homework2.  **Implement ResNet**
  1. Implement Identity block and Conv block. Then build the ResNet50 by stacking these blocks together in Keras (for simplicity)
  2. Highway CNN
  3. Apply model on SIGNS
To run the ResNet, please download ResNet50.h5 file.
This URL might help you, https://github.com/fchollet/deep-learning-models/releases

- Week3
  - Homework1. **Implement of YOLO You only look once.**
   1. Car detection in video
   2. Calculate scores
   3. Filter boxes based on scores
   4. Non-max suppression
   5. Wrap up
   6. Load pretrained model to do detection
       
* Week 4
  - Homework1. **Art Generation with Neural Style Transfer**
   1. Compute the content cost
   2. Compute the styple cost
   3. Total cost and summarization
   4. Optimization and run **interactive session**
 - Homework 2. **Face Recognition and Verification for Happy House**
   1. Verification. Two emcoded pic (128 vector). Use inception model to do encoding
   2. Triplet Loss to create training data set and calculate loss function
   3. Loading trained model. (inception and related)
   4. For each pic, run the inception model on it, and encode it to a 128 vector. So each pic is represented as a 128 vec
   5. Save these vec in a dictionay
   6. By calculate the distance (L2 Norm) and find the smallest dist or say if the dist is smaller than a threshold to tell if we need to open the door.
   
## Course 5 RNN Waiting for release.
