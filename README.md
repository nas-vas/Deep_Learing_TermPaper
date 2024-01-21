# Deep_Learing_TermPaper
 Term paper on Deep learning and reinforcment learning with Q network

New articles and repos - > 

[Atari with gifs](https://github.com/sudharsan13296/Deep-Reinforcement-Learning-With-Python/blob/master/16.%20Deep%20Reinforcement%20Learning%20with%20Stable%20Baselines/16.09.%20Training%20an%20agent%20to%20walk%20using%20TRPO.ipynb)

[more games](https://github.com/shubhlohiya/playing-atari-with-deep-RL/blob/master/README.md)



Main Article: [How to match DeepMind’s Deep Q-Learning score in Breakout](https://towardsdatascience.com/tutorial-double-deep-q-learning-with-dueling-network-architectures-4c1b3fb7f756)

Main code: [DQN](https://github.com/fg91/Deep-Q-Learning)

To create virtual env on mac silicon use [this](https://github.com/conda/conda/issues/12206) 

#### create empty environment

conda create -n py36

#### activate

conda activate py36

#### use x86_64 architecture channel(s)

conda config --env --set subdir osx-64

#### install python, numpy, etc. (add more packages here...)

conda install python=3.6

### Main ideas
The main idea is to start by explaining the history of deep learning and how computer games, whether or not they are related to computers, serve as one of the main building blocks behind new and old deep learning ideas. The first step is to train the agent to play Atari games such as 'Pong' and 'Breakout,' and if time permits, I will explore various Atari and other games.

### Links:
1. [Simple Reinforcement Learning with Tensorflow Part 0: Q-Learning with Tables and Neural Networks](https://medium.com/emergent-future/simple-reinforcement-learning-with-tensorflow-part-0-q-learning-with-tables-and-neural-networks-d195264329d0)
2. [Human-level control through deep reinforcement learning](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf)
3. [Deep Q-Learning Tutorial: minDQN](https://towardsdatascience.com/deep-q-learning-tutorial-mindqn-2a4c855abffc)

### Tips:
To ensure the code works, first, create a virtual environment (venv) with Python 3.6. Install the required packages from the notebook, particularly TensorFlow, as there is an issue with Python 3.7 compatibility. Afterwards, update Python to version 3.7 because Gym won't work on version 3.6. Additionally, upgrade Gym to version 0.21.0 using the command:

pip install --upgrade gym==0.21.0

Due to compatibility issues with the TensorFlow version, use the following import statement:

import tensorflow.compat.v1 as tf
tf.disable_v2_behavior()

There may be a few other minor packages to install, but these errors can typically be resolved with a quick Google search. These dependencies are contingent on the libraries installed previously like this:

conda install tensorflow-estimator=2.1.0

pip install ale_py==0.7

pip install gym[atari,accept-rom-license]==0.21.0

On mac it wont install gym becouse of ' '

pip install gym\[atari\] -> pip install 'gym[atari]' - This is how to install it on mac
