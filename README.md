
# Decentralized Safe Reinforcement Learning for Voltage Control

This repository contains source code necessary to reproduce the results presented in the following paper:
[Decentralized Safe Reinforcement Learning for Voltage Control](https://arxiv.org/abs/2110.01126)  

Authors: Wenqi Cui, Jiayi Li and Baosen Zhang  

University of Washington 


# Motivation
Inverter-based distributed energy resources provide the possibility for fast time-scale voltage control by quickly adjusting their reactive power. The power-electronic interfaces allow these resources to realize almost arbitrary control law, but designing these decentralized controllers is nontrivial. Reinforcement learning (RL) approaches are becoming increasingly popular to search for policy parameterized by neural networks. It is difficult, however, to enforce that the learned controllers are safe, in the sense that they may introduce instabilities into the system.

This paper proposes a safe learning approach for voltage control. We prove that the system is guaranteed to be exponentially stable if each controller satisfies certain Lipschitz constraints. The set of Lipschitz bound is optimized to enlarge the search space for neural network controllers. We explicitly engineer the structure of neural network controllers such that they satisfy the Lipschitz constraints by design. A decentralized RL framework is constructed to train local neural network controller at each bus in a model-free setting.


# Framework for the Decentralized Safe RL Approach
<img src="/RNN.png" height="200px" width="600px" >

# Language and Dependencies
All code are implemented in Python. Data for the power system is imported from MATLAB as 'TestCase33.mat'. We   use   TensorFlow   2.0   framework   to   build   the   reinforcement  learning  environment.

