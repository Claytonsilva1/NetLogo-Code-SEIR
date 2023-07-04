## NetLogo-Code-SEIR

## WHAT IS IT?

This is a simple model illustrating infection spreading in a network with one hundred agents, following a SEIR (Susceptible-Exposed-Infected-Recovered) model.

## HOW IT WORKS

Select the parameters you want to use for the simulation, including the number of edges of the network nodes.

Press the infect button to have a random node infected.

At each subsequent step, there is a probability that each node in gray (susceptible) connected to an infected node becomes exposed and subsequently becomes infected, but also a probability that any infected node will recover with an immunity (which happens when we make the slider prob-susceptible = 0) or after recovery become susceptible again (happens when prob-susceptible > 0).

Thus, we have
### SEIR (Susceptible-Exposed-Infected-Recovered) model: when prob-susceptible = 0 
### SEIRS (Susceptible-Exposed-Infected-Recovered-Susceptible) model: when prob-susceptible > 0.


## HOW TO USE IT

Press...
"setup" to initialize the simulation, creating the network of nodes;
"infect" to infect a random node (necessary for something to happen in the simulation)
"step" to perform a simulation step in which only one time step ("tick") passes
"go" to repeatedly perform simulation steps. (Note that if all nodes turn gray, the simulation continues to count ticks, however nothing else happens since there are no more infected!)

## THINGS TO NOTE/TRY

Make prob-susceptible = 0, then make prob-susceptible > 0 and notice the difference in the graph and the world.


## EXTENDING THE MODEL

1. use a command like "repeat 100 [ layout-spring turtles links 0.2 5 2]" to improve the network layout. To do this, simply uncomment the line before 'reset ticks' in the "setup" procedure. 
2. use the experiment in the 'behavior space' tool, which gives you a spreadsheet with data from 100 simulations with certain variable values.

## NETLOGO FEATURES

Observe o uso dos recursos de rede do NetLogo. Existem muitas primitivas do NetLogo que podem ser usadas para criar e manipular redes, mas é possível criar e usar redes com apenas algumas.

## RELATED MODELS

* One of the related models, and which served as the basis for the construction of this one is Bruce Edmonds' (2013) model. EDMONDS, Bruce. Feb 2013. http://cfpm.org/simulationcourse 

* http://ccl.northwestern.edu/netlogo/models/VirusonaNetwork 

## CREDITS AND REFERENCES

Model by Clayton Ramos, based on the Bruce Edmonds, Feb 2013 http://cfpm.org/simulationcourse
