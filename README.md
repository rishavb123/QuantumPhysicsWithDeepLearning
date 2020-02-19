# Solving the Schrodinger Equation with Deep Neural Networks

Checkout [https://github.com/rishavb123/QuantumPhysicsWithDeepLearning](https://github.com/rishavb123/QuantumPhysicsWithDeepLearning) for the source code and outputs.

The idea behind this project is to speed up the solutions of the Schrodinger equation, an important equation that shows up all throughout quantum mechanics, using a neural network to approximate the solutions that we numerically calculate. I use the Runge-Kutta method to numerically solve the one-dimensional infinite asymmetric well problem for many different potential functions inside the well, and then use a neural network that takes in these potentials as the input and then predicts the energy of the particle in this quantum state and the wavefunction describing the probability of the particle. Another conclusion that we came to see is that the feedforward or the use of the neural network to solve the Schrodinger equation has a more consistent time, staying close to the mean time, or low standard deviation, while the numeric method sometimes took much longer or shorter than the mean time, creating a sense of inconsistency that the neural network solution did not have. 

This project uses data analysis techniques on a few different datasets. The largest of which is the dataset of potentials as inputs and wavefunctions as outputs. We use this dataset to create a predictive model that will approximate the wavefunction solutions of the equation. We generate another dataset by timing the generation and calculation of the solution for multiple potential functions with different complexities. Applying linear regression to this allows me to predict how long it will take to generate data. The final dataset I use is to see the effects of using a neural network instead of numerical methods.

I made this using Google Collab (Python), a hosted Jupyter notebook runtime environment, TensorFlow for the neural network, and a couple more python libraries like matplotlib, numpy, etc.
