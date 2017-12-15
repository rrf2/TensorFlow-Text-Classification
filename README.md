# TensorFlow-Text-Classification
Three different neural network architectures used for classifying text: a recurrent neural network, a recurrent neural network altered to have longer lasting state memory, and a feed forward neural network . 

The code is currently written to perform classification on 3 specific texts, but can be easily altered to perform classification on any number of texts.

The basic recurrent neural network performs poorly due to the vanishing gradient problem. The altered recurrent neural network solves this problem by not only remembering the state for the next step in the network, but also for the step 10 steps ahead. This allows the number of steps needed for the gradient to make its way through the network during backpropagation to be reduced by a factor of 10.

The feedforward network performs the best, but cannot accept an input of arbitrary length, unlike the recurrent neural network model.
