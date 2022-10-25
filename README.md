# DQN-learn-pong
Using Deep Q-Learning Networks (DQNs) with reinforcement learning to train models to play pong. Where the only input into the deep neural networks on pre-processed screenshots from the game and reward information based on scoring or conceding a point. I test multiple versions on the learning networks, from a standard DQN, to a Double DQN and then both of these with a dueling architecture added on top.

## First Episode of Learning ---> Final Episode of Learning
The paddle on the left is controlled by the rules-based computer and the paddle on the right is controlled by the DQN trained model.

![NDQN_Pong_Ep_0](https://user-images.githubusercontent.com/113981071/197782949-fcb95877-61da-4541-acc6-e5e7bc35d936.gif)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![NDQN_Pong_Ep_19](https://user-images.githubusercontent.com/113981071/197783047-ae14cf6f-ddcf-4e8f-9930-8d2ec4c8be11.gif)

These videos are end of episode recordings for the standard DQN with no Dueling model. We can see that after the initialisation episode the model does not yet know what to do and quickly gets stuck at bottom of the screen until the game ends. Then after the final episode the model has clearly learnt the best strategy for the game based on the same static start point. A more dynamic start would likely require much more training.

## Evaluation

Training and testing graphs showing the total reward gained from the models, with some models clearly optimising faster than others.

<img src="https://user-images.githubusercontent.com/113981071/197786807-c55960f6-82e9-4e78-95c7-0c295a7d784b.png" alt="traininggraph" width="500"/>
<img src="https://user-images.githubusercontent.com/113981071/197785385-7e4fbd45-9d9e-4f3a-831d-74ae49de8d56.png" alt="testinggraph" width="500"/>


