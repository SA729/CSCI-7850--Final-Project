# CSCI-7850--Final-Project

Mathematical models are an becoming increasingly powerful tool in
cancer biology to understand the complex interactions between 
the immune system and the tumor. Numerical approximation methods are commonly 
used to solve and simulate the tumor-immune dynamics. These methods rely on the discretization and hence, solutions are discrete or have limited differentiability. Growing evidence suggests that neural networks provide more accurate and precise information about tumor-immune dynamics. In this work, we use a neural network to solve and simulate the nonlinear ordinary differential equation based tumor immune model and we compare the results with numerical solutions based on Runge-Kutta 4 th order method.

 We have attempted to solve a effector cells and tumor cells interaction model developed by Kuznetsov et al. using a neural network technique first proposed by Lagaris et al. and comparing the solutions with Runge-Kutta 4 th order numerical approximation method for 5 days and 10 days period. 

In this work, a fully connected neural network(FCNN) with  3 hidden layers and 32 nodes per each hidden layer, with the
activation function of tanh were used for each dependent variable( tumor cells and effector immune cells). One input unit were used to represent the independent
variable time(t). Two fully connected neural networks were used to represent two dependent variables, tumor cells and effector cells in the model.  The hyperparameters of this FCNN are optimized using Adam, with a learning rate of 0.003 and training rounds of 3000. We made use of NeuroDiffEq python library to solve the tumor -immune model in this project. 
