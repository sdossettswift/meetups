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
- style transfer -- ie, things like waterlogue - make a selfie look like a vangogh painting

### tensor flow - 
- variables
- sizing 
- memory matters -- limiting agent
- batch up data 
- pooling layers - simplifies images (pulling or polling>)
- flatten layers - fully connected layers
- run things on a subset and then move to bigger dataset, eventually up to the full kahuna -- again, it is an iterative process 
- 

### style transfer-
- mxnet (www.github.com/dmlc/mxnet)
- style score - looks at correlations of features 
- (!!!)
- mxnet is pretty powerful, fairly fast
- small community, but high performing 

### recurring neural networks (RNN)
- takes results of weights, feeds it forward, discovers context
- the unreasonable effectiveness of rnn (google this famous blog post)
- assign numbers to words, evaluate sums for sentance structures, etc.  
- keep the model from forgetting 
- separate state in memory allows for remembering 
- example makes use of tensor flow -- tensor flow is a good place to start b/c it makes things relatively simple 
- example generates a (gibberish) version of a tv script modeled after a simpsons script

### reinforced learning (!!!) 
- guy is really interested in this field.
- similar to closed loop systems
- three approaches:
	- supervised learning
	- reinforeced learning 
	- unsupervised learning 
- in reinforced learning - there are observables, rewards, actions. the training: reqw version of a tv script modeled after a simpsons script

### reinforced learning (!)
- rewards!! 
- tries to make it work 
- close to engineering
- hal 3000 - (my opinion: seems like it is cut loose)

### generative adversarial network 
- guru trying to fool training model, using bad data
- stone sharpening stone 


# libraries:
- mxnet
- pyTorch - academic
- theano - low level
- blocks - high level
- keras - built on top of theano
- tensor flow - good starting point, huge community, google, will incorporate keras
- second learning - general ml techniques 

## web apis
- microsoft azure ml
- google ml
- amazon ml
- ibm watson - conversation`
- wit.ai: langauge, similar to alexa, google home, homepod
- api.ai
- diffbot : claims to parse language as well as google

* feed these data and watch them go

### a.i. experiements: thing translator (youtube)
- cloud vision + translate api

## resources:
- linear digressions podcast
- twiml & ai
- the talking machine
- data skeptic
- moocs - udacity
- youtube: andrwe ng(standford), andrew karpathy, siraj raval
- techincal blogs
- blogs
- free books -> check out his slides for all links
- udacity example repos are available 

### predictions
- web3.0
 -backend data - google is going to be the internet 
- everything else is just goign to be a datasource
- query based interface only - no separate websites, apps
- melding of online content/real surroundings/ads

- stock market
	- short term:ml palyers will become incredibly wealthy  investors will rely on ai fund managing bots
	- long term: AI will det exact value of a company 


