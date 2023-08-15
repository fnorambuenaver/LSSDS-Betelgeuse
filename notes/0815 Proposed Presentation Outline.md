Proposed Structure for the Presentation:  

# 1. Introduction: Theoretical background about our topic
1. What are radio signals
2. Different classifications and the importance of identifying the different types of radio signals.
3. The instrument used to observed these radio signals.

# 2. Objectives:
General:
Performing classification of radio signals through the implementation of Deep Learning architectures.
### 2a. Specifics:
- Understand the theoretical part of the project
- Implement different DL architectures
- Modify the hyperparameters and compare other DL architectures in order to obtain the higher accuracy possible.
	- keras-tuner

# 3. Description of the DL architectures implemented:  
Into what architectures were used
		a. CNN  (Convolutional Neural Network)
			 - comparing a Fully Connected NN with a CNN, 
			 - the amount of parameters of two layers
			 - the need to maintain spatial information
		b. AlexNet
		c. ResNet
			 - The concept becomes necessary when introducing too many layers to overcome the vanishing gradient
		c. Wide ResNet  
			 - Use residual blocks and layer features as if we were building a wide neural network with neurons
		d. SENet  (Squeeze and Excite)
			 - Implement the ability for the model to create an excitation vector to shutdown entire features layers and excite others

## 3.b Experimentations with Data Preprocessing
- PCA
- FFT2D

## 3.c Transfer Learning Candidates

# 4. Results obtained from using the different architectures  
Comparing 
- test accuracy
- precision
- recall
- training time
- Number of parameters
- programming complexity

As an example share:
	a. Plots  
	b. Accuracy  
	c. Confusion Matrices  

# 5. Conclusions
