## Stochastic Channels CP project

Channel models can be instantiated directly
from state diagrams simply by keeping track of the state of the channel
and allowing stochastic changes of state to occur at appropriate transition
rates. If the model is updated in short time steps of duration delta_t, the probability that the channel makes a given transition during an update interval
is the transition rate times delta_t.

### TODOS/QUESTIONS (as of Jan 20th)
- Chow, how we calculate the probability that a channel changes state and the calculation of the probability of going to another state?
- Should we implement more advanced model, if yes how to approach it and choose the model?
- 

### TODOS/Questions: (as of Jan 16th)
- [ ] variance should be calculated at the stationary phase (doesn't make sense in the beginning)
- [ ] do the same for sodium NA
- [ ] Change the structure of the code so that at each time step the whole population is being considered
- [ ] Clean up the code, add documentation and intro
- [x] 2 plots of the variances going down


---------------------------------------------
### TODOS/Questions: (as of Jan 9th)
- What are the values for conductance and Reversal potential? K values?
- 0) Simulate a two state system
- 1) Start by fixing the voltage
- 2) Introduce time! But how? small delta_t
  - safe way to do it is by choosing delta_t 
    according to the largest alpha/beta we can have 
    (largest voltage)
- Compare the temporal mean of stochastic ion channel
  at a fixed voltage with stationary value of n** at same V4 (from HH)
- Meet every Monday (at 3PM)

