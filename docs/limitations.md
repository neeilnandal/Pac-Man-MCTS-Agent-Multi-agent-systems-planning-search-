### Limitations

- **Short-term Heuristic Bias:** Our heuristics were designed for short-term goals (gain food, stay away from ghosts, bring home food if needed). MCTS typically works well when it can find its own path to long-term objectives (winning the game).
  
- **Computational Constraints:** One simulation using the full 1200 game steps takes up to one minute and is typically not very informative, limiting our ability to use longer roll-outs.

- **Manual Weight Tuning:** The feature weights were largely determined manually, which is a sensitive process. Slight changes in weights could significantly impact performance.
