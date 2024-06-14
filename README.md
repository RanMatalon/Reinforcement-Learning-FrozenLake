# Reinforcement-Learning-FrozenLake

In this project I present several algorithms in reinforcement learning for the convergence of a value/policy function in the frozen lake game.

Policy vs Value iteration discussion:

It's clear that Policy iteration takes less iterations to be evaluated (for same theta) - 9 comapring to 119 in value iteration.
While policy iteration needs less iteration to converge, it is clear that its' iterations by far more expansive than the value one - 0.001 secs for policy, 0.0005 for value (doubled).

Monte Carlo vs Sarsa vs Q-Learning discussion:

We could see that Monte Carlo rarely and barely converges, that means it rarely gets to the Goal with the decaying epsilon.

![image](https://github.com/RanMatalon/Reinforcement-Learning-FrozenLake/assets/138029692/99f74d53-2fc1-4189-baf7-1eb5a0f0719c)


On the other hand, Sarsa converged to any epsilon >= 0.4, which shows that monte carlo didn't has good exploration. The convergence is still not to optimal values.

![image](https://github.com/RanMatalon/Reinforcement-Learning-FrozenLake/assets/138029692/ccbd1fb7-ad45-4630-bde7-a71afd333be6)

Q-Learning, in contrast to Sarsa's randomness on the next state, for any state, learns the maximum reward of the next state without its randomness, making it to converge to optimal values.

![image](https://github.com/RanMatalon/Reinforcement-Learning-FrozenLake/assets/138029692/97fe1369-b0a8-4209-ba7b-63fb654b6d24)
