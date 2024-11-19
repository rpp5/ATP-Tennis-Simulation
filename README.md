# ATP-Tennis-Simulation:
This project aims to assess the state of a ATP tennis match through a Monte-Carlo based simulation approach that takes into account each player's serving and returning ability from any scoreline. 

### Step 1: Compute P_a - the probability of the server winning a point (which will be useful when utilizing a Markov Chain Model) based on both their serving ability and the opposing player's returning ability: 

### Step 2: Run Markov Chain Model
<img width="756" alt="image" src="https://github.com/user-attachments/assets/8f0bc5f5-ad1b-48b4-b418-adac1d5c83b7">

## Features:

1) The first feature this model calculates is **win probability**, which simulates a tennis match from a predetermined scoreline and gives the percentage of times those simulations ended in a win for a specific player.
2) The second feature this model calculates is **leverage**, which is the difference in win probability depending on whether a player scores or does not score -- essentially leverage aims to quantify the "importance" of a particular point in the match by looking at what the win probabilities would be under two different realities.

## Sample Match: Roger Federer vs Rafael Nadal (2008 Wimbledon)

To display and test my findings, I calculated win probability and leverage at every point in the Roger Federer vs Rafael Nadal 2008 Wimbledon Final epic that went into 5 sets and was extremely close. The results are in the 'new_tennis_sim.ipynb' notebook.

## Further Study and Applications:

While the model is quite simple, the power of simulation is immense and this model has wide applications to sports betting. I'm looking to factor in head to head record as well as momentum in the model.
