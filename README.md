# RLLNESG
Reinforcement Learning for Learning Nash Equilibrium in Strategic Games

YouTube Discussion: https://youtu.be/CrQFyXsb10c?si=cZVTELPpmcIK9a5m

## **Execution instructions**

1. Save the YAML file as env.yml in your project directory.
2. Run the following in directory with yml.
```conda env create -f environment.yml```
3. Run the following:
```conda activate open_spiel_env```
4. Install and open Jupyter
```pip install notebook```  
```jupyter notebook```
5. Run test.ipynb in Jupyter 

## **Problem statement** 

I propose applying reinforcement learning (RL) algorithms to strategic normal form games to test how well, or if at all, RL agents can converge onto the theore;cal equilibrium for a game. I want to iden;fy the following:
1. Which RL algorithms can converge onto Nash Equilibrium for a game.
2. How explora;on vs. exploita;on balance affects Equilibrium convergence.
3. How do different RL algorithms perform against each other in the same game.

## **Codebase** 

The OpenSpiel environment contains mul;ple strategic games, such as Prisoner’s Dilemma, where two agents can play against each other. In contrast, the OpenAI Gym environment mostly contains single player, control focused games, such as Lunar Lander. Therefore, I believe that OpenSpiel will provide the beRer codebase for my proposal than Gym.
I would supplement this with the standard Python data science libraries – Matplotlib, Numpy, and Pandas – to perform data analysis and visualiza;on as needed.

## **Project Plan**
1. Sequences: I will incorporate iterated game playing in my analysis. Therefore, instead of just playing one-off Prisoner’s Dilemma games, I would have the RL agents paly against each other repeatedly.
2. State space: The state space for each game will be the current moves available to the agent and the past moves knowledge.
3. Action space: The moves available to an agent – cooperate or defect.
4. Transition and reward functons: I will use the literature standards for these func;ons.
5. Baseline: I will compare the RL agent performance against random selec;on of coopera;on vs defec;on. Random move selec;on is the simplest result I can generate therefore I will start there.
6. Stretch goal: If possible, I will try to play the game with more than 2 agents to see how coopera;on occurs within a team rather than an individual.
