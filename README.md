# reinforcement-learning
This repo is for all my RL related stuff

### RL_CartPole_v1.ipynb
In this notebook, I discover reinforcement learning by following the example of the book Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow by Aurélien Géron.
The example used here is CartPole-v1 (Gym library) where a cart can be pushed left or right in order to keep an attached pole in balance.
First I test a hard-coded policy:
- The cart will be pushed to the left, if the pole is leaning to the left and right if it leans to the right.
This policy isn't a good choice, as it only achievs to keep the pole upright for max 62 steps
The second implemented policy is the REINFORCE algorithm out of the policy gradient (PG) class:
- Basically a neural network policy will be trained here. Each action is getting discounted here in order to weight the actions that lead to an outcome.
Here we get a mean reward of 174.6 which means, that we are able to balance the pole for that many steps in a row.
