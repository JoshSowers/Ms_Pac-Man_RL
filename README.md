# Playing Ms. Pac-Man using Reinforcement Learning

##Summary
In this repository, the goal was to use Deep Q-Learning in order to have an agent learn to play Ms. Pac-Man using screen images. As such,
a convolution neural network was used to analyze images of the screen that were preprocessed and stitched together.The environment was 
sourced from OpenAI gym. The agent was trained and the network weights were saved at interval in order to preserve the network and allow
for training over multiple days. Training was conducted over a series of days using Google Colab free GPU. Only small incremental changes
were observed during this brief training period, however there was a noticeable difference in performance (~280 to ~450), with the agent 
reaching higher scores more often than during the beginning of training. That is, the agent was found to achieve scores in the 1200 range
more often, suggesting that the agent had learned one area of the environment and was able to exploit that area when it found itself there.

##Files
The .ipynb file contains the entirety of the code from defining the class for the agent, preprocessing, and then executing training. The
agent is stored as a .h5 file named 'agent'. A short video of the agent playing Ms. Pac-Man can be found in the .mp4
