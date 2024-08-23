# Taxi_dropoff
OpenAI Gym Taxi dropoff reinforcement learning problem.
Overview Drive a Taxi Using OpenAI Gym.

Reinforcement learning has come a very long way, many people use it for different things, including games and others.

OpenAI Gym: This provides virtual environments for developing and testing learning agents for deep learning models.

Project: This is a reinforcement learning simulation where an agent, in this case a taxi navigates an environment, a grid world to pick up and drop off passengers using the least moves. The goal is to be able to navigate the environment efficiently while minimizing penalties and maximizing rewards. The simulation would be rendered as an RGB array using matplotlib.

Rendering: Visual representation of the work. In this case an RGB array showing the state of the environment. Environment: This is a simulated environment where an agent interacts, takes actions and receives feedback. Feedback: Reward, Penalty, Done, New State. Location: Four locations are mapped out Red, Green, Yellow, Blue (south, north, east, west). State: This is; Taxi location, Passenger location, Destination location. States are represented as tuples (array of values) which describes the environment. Actions: This is what the taxi can do; directions(locations) it can move, pick up passenger and drop off passenger. The taxi can perform six actions. Rewards: Successfully dropping off a passenger at the designated point. Penalties: Every move it takes, picking up or dropping off at the wrong points. Reward of -10 = 1 penalty.

Algorithm Used: Q-Learning. Qlearning is an algorithm that helps a learning agent to maximize the total reward over time through repeated interactions with the environment, even without the model of the environment.

Exploration: The agent explores the environment by taking random actions and observing the resulting states, no learning or policy optimization is performed.

Exploitation: The agent chooses actions that it will give the highest expected reward based on learnt knowledge or optimized policy. This is done after the agent initial learning phase (exploration).

Epsilon Greedy function: With probability(epsilon), the agent explores by selecting a random action otherwise, the agent exploits by selecting the action with the highest Q-value. Q-value: Values in the Q-table. Q-table:A lookup table where we have the expected future reward of each action taken in a state, initialized with zeros at the start of the program.

PS: Tesla and automated drones uses this technology.
