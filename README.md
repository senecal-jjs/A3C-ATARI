# A3C-ATARI
Asynchrounous actor-critic reinforcement learning implementation. 

This implementation borrows heavily from https://github.com/dennybritz/reinforcement-learning

## Running the algorithm 
python train.py --model_dir /tmp/a3c --env Breakout-v0 --t_max 5 --eval_every 300 --parallelism 8

+ --model_dir specifies the save directory for checkpoints, videos, and results
+ --env specifies the ATARI game environment
+ --t_max specifies the number of steps an agent will take in an environment, before accumulating and 
    applying a gradient update
+ --eval_every specifies the number of seconds in between evaluations of the global policy
+ --parallelism specifies the number of worker threads (i.e the asynchronous part of the actor-critic algorithm)
