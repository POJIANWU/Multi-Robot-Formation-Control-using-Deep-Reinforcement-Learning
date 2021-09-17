# Multi-Robot-Formation-Control-using-Deep-Reinforcement-Learning


In this project deep reinforcement learning is used to train multi-agent robotic systems to perfrom leader-follower formation control . The OpenAI's MADDPG project is used after modification to train the agents.

## Framework

The Framework used in this thesis is Python 3.6.9 installed on Ubuntu 18.04 LTS. Along-side with Numpy which is a python library that provides dozens of methods to manipulatethe multi-dimensional arrays and matrices that could be helpful in Mathematical calcu-lations, more about the library can be found at NumPy Website.  Tensorflow library isalso used which is a free open-source library for Machine Learning developed by Googlethat facilitates the training of the deep neural networks.

<p align="center">
  <img  src="https://user-images.githubusercontent.com/42684592/123695973-82063300-d85b-11eb-8349-84dadbda6b69.png">
</p>


## Environment

The  environment  is  the  single  most  important  element  in  the  Reinforcement  Learningprocess since it presents the physical world that the agent interacts with.  In this thesisthe environment used is Multi-Agent Particle Environment based on OpenAI work. OpenAI is artificial intelligence research laboratory that develops free open-source toolsand libraries that helps the Artificial Intelligence developers community in the Researchand Industry field.The original environment is a 2D world with a continuous observation and discreteaction space, along with some basic simulated physics.  It was developed such that theagents are divided in 2 groups: Good Agents, Adversary Agents, in which the good agentstry to cooperate to cover certain goal landmarks so that the adversary agents can notcover these goals.Many modification are made to this environment in the thesis so that it can be usedin the Leader-Follower Formation Control favor, including:

1.  The agents are divided into:  One Leader Agent, Two Follower Agents.
2.  The goal is an individual landmark its location is fixed, unlike being assigned ran-domly  in  the  original  environment,  in  the  left  down  corner  of  the  environment,specifically at location (-0.8, -0.8) with respect to the coordination plane which hasa center of (0, 0) right at the middle of the screen.
3.  The landmarks representing obstacles are assigned randomly.
4.  All of the agents initial positions are assigned randomly constrained to be at thefirst quadrant of the coordination system unlike being completely random at theoriginal environment.
5.  The maximum speed of the agents is set to 0.2 unlike the original environments6.  The size of the agents is reduced and the landmarks size is magnified compared tothe original environment.


<p align="center">
  <img  src="https://user-images.githubusercontent.com/42684592/123695976-829ec980-d85b-11eb-8d5f-a7f1391d9418.png">
</p>