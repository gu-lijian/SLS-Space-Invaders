# SLS-Space-Invaders
Using DQNetwork implementation for reinforcement learning on game space invaders

# Run with per trained model
- Please make sure below command is release in notebook file and configure the corresponding model file.(In this project we provided 4 pre trained model files with 2k, 10k, 50k and 1m training steps)
- dqn.load_weights('SavedWeights/1m/dqn_weights.h5f')
- Please also ensure below command is commented
- dqn.fit(env, nb_steps=50000, visualize=False, verbose=2)

# Train from a pre trained mode
- Please assign pre trained model file name to variable pre_trained_model (In this project we provided 4 pre trained model files with 2k, 10k, 10 0k and 1m training steps)
- Uncomment below command to ensure load this pre trained model
- dqn.load_weights(pre_trained_model)
- Please uncomment below command for training based on a pre trained model
- dqn.fit(env, nb_steps=50000, visualize=False, verbose=2)

# Notes
If you meet any model related error, please uncomment code "del model” and run from there once again , it will solve the problem.

# Optional
You can set visualize=True when running testing command as below. When visualize=True the speed of testing will be slower than without visualization of the game.
scores = dqn.test(env, nb_episodes=100, visualize=True)
