# Using Traditional Q-Learning on the Mountain Car environment

## Summary
In the notebook found here, I use traditional Q-learning to train an agent to learn the Mountain Car environment from OpenAI. The influence
of different global parameters was explored including learning rate, discount factor, and decay epsilon/minimum decay for an epsilon greedy
strategy. The results found were as expected. 

A lower learning rate led to larger changes made by the agent, which allowed for the quickest but least stable learning. As the learning 
rate increased, it took the agent longer to learn the environment, however the learning was much more stable. 

For discount factor, the larger the discount factor, the more the agent will prioritize long term rewards. This plays out as expected with
the largest discount factors giving the most long term rewards and the smaller discount factors resulting in high amounts of variability.

Epsilon controls the explore vs exploit relationship of the agent. In this example, the values of epsilon and minimum epsilon were varied
to examine how different decay rates would affect the explore vs exploit relationship. What is seen is that large initial exploration rates
with no minimum epsilon values led to better learning over time compared to fixing a minimum exploration rate of 25% or 50%. In this 
example, the random action taken is actually 1-epsilon, which means that lower values of epsilon led to a higher amount of exploration and
higher epsilons led to more exploitation.

## Files
All code can be found in the .ipynb file. 

