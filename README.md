# Neutron_MonteCarlo_Simulation
In this project, I used a Monte Carlo simulation to estimate the critical mass of uranium-235 by modelling neutron-induced fission. The aim was to determine the size at which a self-sustaining chain reaction occurs.

I began with a simplified one-dimensional model, representing uranium as a line of length . Initial fission events were generated at random positions, and each produced neutrons that travelled either left or right. I tracked whether these neutrons remained within the material and caused further fissions, allowing me to count the number of secondary events. By repeating this process many times, I calculated the average number of secondary fissions per initial event.

The model was then improved by introducing randomness in the number of emitted neutrons and more realistic diffusion behaviour. I varied the length L to identify the critical value where the reaction becomes self-sustaining.

Next, I extended the simulation to three dimensions, modelling uranium as a cube. Neutrons were emitted in random directions using spherical coordinates, and their travel distances were sampled from a probability distribution. I calculated new positions for each neutron and checked whether they remained inside the cube to continue the chain reaction.

Finally, by varying the cube size and analysing when the number of secondary fissions stabilised, I estimated the critical volume and corresponding critical mass using the known density of uranium. This demonstrated how Monte Carlo methods can model complex physical systems that are difficult to solve analytically.
