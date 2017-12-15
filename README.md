# RevEngg_Policy

The IPython notebook provides a tabular Q-learning algorithm for OpenAI FrozenLake8x8 Environment. 
The environment is modified so to make the actions determinstic. 
This functions as a deterministic policy, gridworld environment.

Prerequisites: OpenAI Gym
The installation instructions can be found here: https://github.com/openai/gym

To find the optimal forward policy, execute the RevEngg_pol.ipynb as is.

For the reverse policy, modify the following file in your gym source folder :-
.../python2.7/site-packages/gym/envs/toy_text/frozen_lake.py

  Change the 8x8 map by swapping the positions of 'S' and 'G'
        "SFFFFFFF",               
        "FFFFFFFF",
        "FFFHFFFF",
        "FFFFFHFF",
        "FFFHFFFF",
        "FHHFFFHF",
        "FHFFHFHF",
        "FFFHFFFG"
        
        changes to
        
        "GFFFFFFF",
        "FFFFFFFF",
        "FFFHFFFF",
        "FFFFFHFF",
        "FFFHFFFF",
        "FHHFFFHF",
        "FHFFHFHF",
        "FFFHFFFS"
        
Execute RevEngg_pol.ipynb to find optimal reverse policy 
