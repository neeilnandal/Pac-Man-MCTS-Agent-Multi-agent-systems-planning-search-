## Results

The results of the first experiment, which was conducted as an ablation study beginning with the baseline implementation, are presented in Tables 1 and 2. We incrementally added features and tested multiple values for each feature. Overall, every implemented feature contributed positively to the heuristic function, as reflected by the increase in ELO scores relative to the baseline across all configurations.

For the defensive agent, introducing a reward for remaining near its own food improved the robustness of the agent, after which it did not lose any matches. Based on the ELO scores, including those of the opponent, the values of -0.001 for total Food Distance and -0.1 for closest Food Distance appeared to perform best. We also observed that overly large values caused the agent to focus less on pursuing enemies, which is its primary objective. For this reason, slightly smaller values were preferred.
