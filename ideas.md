### IDEA NR.1
Use reinforcement learning(either DQN, A3C, PPO or something else...) to directly optimize the weights of a model of an agent or an standalone model(like an convolutional neural network for Dog breed classification).
Like in https://arxiv.org/abs/2001.09212 the optimization algorithm(the RL algorithm) will move over the weights(the weights will be represented like tiles) and the avaiable actions will modify the weights in place.
In other words: the optimization agent will move over the weights tiles in different directions and will either modify the weight/weights in place or move to another weights tile until the target score/value is met.
The RL agent can choose between the following actions: move to direction(where the direction is defined by the dimension of the weigth tensor, in a 2D weight tensor the actions are go UP, DOWN, LEFT, RIGTH), replace or modify weight value(the weights will be modified with discrete variables/values like modify the weight value by adding/substracting/multiplying the number 1 or 0.5 with the weight value)
The RL optimization agents will be nested, so the first RL agent/model optimizes the weights of the seconds RL agent/model who will optimize the weights of the next agent/model, until the last agent/model is the final target of the optimization and as such is directly used in an environment or program.

  
