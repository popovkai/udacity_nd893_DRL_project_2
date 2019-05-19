#  Project Report

For this project, I only work on the "first version" requirement which contains a single agent.

This project implements an DDPG agent [paper](https://arxiv.org/pdf/1509.02971.pdf).

NN info:

- Two identical neural network configurations for both Actor and Critic.
- It contains 2 fully connected hidden layers (FC) followed by ReLU none-linear activation layers.
- Also add batch normailzation during training.

Parameters used in DDPG algorithm:

- Replay buffer size = 10^5
- Minibatch size = 128
- Discount factor = 0.99
- Soft update of target parameters = 1e-3
- Learning rate of the actor / critic = 2e-4
- L2 weight decay = 0

## Result

```
Episode 100	Average Score: 3.55
Episode 200	Average Score: 23.62
Episode 244	Average Score: 30.01
Environment solved in 244 episodes!	Average Score: 30.01
```

## Future Works

1. Get my machine running !! I still don't like coding at Notebook. I like vi.
2. Different hyperparameters (LR, different optimziers, epsilon)
3. Different NN configurations - current NN is not deep at all
4. Try the multi-agent version
