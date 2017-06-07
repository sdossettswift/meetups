# PyWeb Houston: Introduction to Machine Learning 
## Digital Crafts | Room 47

Guy de Carufel 
- gh: @carefulguy

- deep  learning 

### ai vs ml cs dl 
- ai - helping computers be smart - since 1950s
- ml - a method for ai
- dl - ml techniques based on neural networks - mostly academic since 90s, has been taken seriously as a practical solution during the past 6/7 years
- - deep learning careers are pretty novel - dl engineers
- dl - all the hype right now b/c computing power
- rice u - made announcement regarding hashing - makes ml/dl a lot more accessible -- increases training speed by like 95-99% (!!!)
- goolge tensor flow - training for neural networks
- new applications: self driving cars, drones, real time lang translation, art/music generation, ai in VR | gaming 
- ml can learn to play games so well, no one can beat it
w

## basic steps 
1. get data 
1. clean it up, prepare & manipulate
1. train model (design, build, train, give expected outcomes, adjust until you are there) - iterative process
1. test data
1. improve 


## neural networks
- inputs : features (color, features, etc.) 
- lines connect features, weights are the intersections between nodes 
- input layer ---> hidden layer ----> output layer
- deep  neural network - add layers - create dimensionality 
- pattern recognition!! 
- alpha go -- 16 layers deep - massive scale  - scale rivals mouse brain

### technical challenges 
- getting the right data
	- google has a huge advantage b/c htey have so much data
	- training set (80%), validation set (10%), testing data (10%)
	- hyperparameters -variables 
	- pulling -- manipulating importance of weights
- model architecture  - fully connected neural net 
- scaling -- aws or some other cloud service b/c it will eat your gpu
- feature engineering: picking the right data 
- saving an re-use of trained models -- you want them specific enough to give you meaningful info, but the more specialized it gets, the more limitations (obviously)


### linear regression 
- making use of a neural network to make a specific quantitative prediction
- see the code on gh - Udacity - deep learning 
- carefulguy/udacity-dlnd-neuralnet https://github.com/carefulguy/udacity-dlnd-neural-net

#### training models
- forward propogation vs backward propogation 
- going backwards and forwards, you can update the weights, iterate over and over until the predicitons are super close to your actual values. 
- https://github.com/carefulguy/udacity-dlnd-neural-net/blob/master/dlnd-your-first-neural-network.ipynb
- eventually, you reach a floor where there are no marginal gains in fine tuning 
- as you continue training, you will run into the problem of overfitting -- the
- basically -- trying too hard 

### looking at info
- look at data and see if there is a factor you didnt train for (christmas, holiday, etc)

## cnn - convolutional neural network
- pixels 
- patterns become features
- computer vision 
- image classification || style tranfer 
- it gets increasingly complex 

:



