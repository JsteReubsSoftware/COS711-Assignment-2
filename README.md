# COS711-Assignment-2

In this assignment we conducted a comparative study by comparing three different optimization algorithms for solving the Almond Classification problem. Our three algorithms are:
- Stochastic Gradient Descent (SGD)
- Adaptive Moment Estimation (Adam)
- Resilient Backpropagation (RProp)

Additionally, we tried to enhance the predictive power of a NN model by implementing a Hybrid Learning approach.

### How the Hybrid Learning Approach works:
1. We use all three algorithms to setup a NN model using exactly the same architecture for all models.
2. During the training phase each model trains separately and we collect the gradients for each algorithm and store it in a vector.
3. After each epoch we take the average of all three algorithms' gradients.
4. The average gradient is then used to update the weights of one of the three NN models.
5. The process continues until the training phase is complete.
6. We then use the hybrid trained model to make predictions on an unseen dataset and evaluate its performance.
