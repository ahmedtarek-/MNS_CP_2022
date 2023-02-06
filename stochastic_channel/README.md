## Stochastic Channels CP project

Channel models can be instantiated directly
from state diagrams simply by keeping track of the state of the channel
and allowing stochastic changes of state to occur at appropriate transition
rates. If the model is updated in short time steps of duration delta_t, the probability that the channel makes a given transition during an update interval
is the transition rate times delta_t.


### TODOS/Questions: (as of Feb 6th)
- Get the mean working better (increase the number of channels)
- Why the varying voltage fucks up the behaviour (is it a bug?)
- Decide on plots to use for presentation
  - The 1, 10, 100 channels plot
  - The mean and variance graphs

### TODOS/Questions: (as of Jan 23th)
- Plots 
  ![plots](https://user-images.githubusercontent.com/10937709/214603721-7174aad6-33af-45c7-8841-a979634b420f.jpg)
  - The idea is to plot the mean of n and m for a fixed population agains different voltages (to make sure the channel dynamics are right)
- HH model (using fraction of open channels instead of n4 and m3)
- ISI based on HH model? (if we have time)

### TODOS/Questions: (as of Jan 16th)
- 2 plots of the variances going down
- variance should be calculated at the stationary phase (doesn't make sense in the beginning)
- do the same for sodium NA
- Change the structure of the code so that at each time step the whole population is being considered
- Clean up the code, add documentation and intro


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

