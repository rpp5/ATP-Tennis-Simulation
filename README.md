# ATP-Tennis-Simulation:
This project aims to assess the state of a ATP tennis match through a Monte-Carlo based simulation approach that takes into account each player's serving and returning ability from any scoreline. 

### Step 1: Compute P<sub>a</sub> - the probability of the server winning a point
To compute P<sub>a</sub>, we have to take into account the skill of the server, but also of the returner, as stronger returners will lead to a lower probability of the server winning a point. If we suppose the first serve is in play, then let P<sub>s</sub> = P(Server wins his first serve (in isolation)) and P<sub>r</sub> = P(Returner wins point when returning first serve (in isolation)). Such data can be found on atptour.com. Then the final probability of the server winning a point on his first serve is $\frac{P<sub>s</sub> + (1-P<sub>r</sub>)}{2}$

### Step 2: Run Markov Chain Model
<img width="756" alt="image" src="https://github.com/user-attachments/assets/8f0bc5f5-ad1b-48b4-b418-adac1d5c83b7">

## Features:

1) The first feature this model calculates is **win probability**, which simulates a tennis match from a predetermined scoreline and gives the percentage of times those simulations ended in a win for a specific player.
2) The second feature this model calculates is **leverage**, which is the difference in win probability depending on whether a player scores or does not score -- essentially leverage aims to quantify the "importance" of a particular point in the match by looking at what the win probabilities would be under two different realities.

## Sample Match: Roger Federer vs Rafael Nadal (2008 Wimbledon)

To display and test my findings, I calculated win probability and leverage at every point in the Roger Federer vs Rafael Nadal 2008 Wimbledon Final epic that went into 5 sets and was extremely close. The results are in the 'new_tennis_sim.ipynb' notebook.

## Further Study and Applications:

While the model is quite simple, the power of simulation is immense and this model has wide applications to sports betting. I'm looking to factor in head to head record as well as momentum in the model.
