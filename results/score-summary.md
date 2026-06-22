We’ve looked at many different hyperparameters and heuristic evaluation func
tions. Our most significant result was the impact of the desireToHome function
in the offensive agent and the distanceToFood for the defending agent. Where
we first determined all values by ablation study using heuristic agents, we saw
that these values were not exactly transferable to using with our MCTS agents
and required some manual adaptation by observation. The planning nature of
MCTSmaybe influential to the performance compared to the reflexive heuristic
agents.



Our heuristics were actually designed for short-term goals: gain food, stay
away from ghosts, bring home food if needed. However, MCTS typically works
well if it could find its own path to long-term objectives (win a game). This was
actually due to time restrictions hard to implement as typically games would
run for 1200 steps. One simulation using 1200 steps already takes up to one
minute and is typically not very informative.
After having our heuristics fine-tuned for MCTS, we saw very good behaviour
9
for the MCTS against the baseline agents: a win-rate of 98% and ELO-scores
of over 1600. Letting it play against a reflexive agent with the same heuristics
showed however that the heuristics were the power of the algorithm- and not
the MCTS itself.
