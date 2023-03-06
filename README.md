# special-dominoes-model
## WHAT IS IT?

This project simulates the tumbling of a random arrangement of dominoes when a select few are fallen. The behaviour demonstrated here can be similar to propagation in a network from select starting source(s).

## HOW IT WORKS

For simplicity, we deal with dominoes with special properties. The dominoes contain parts (4 or 8 depending on user choice), which fall in respective directions instead of one piece falling on its side on one direction.

With the above in mind, we assume a perfectly flat surface, where only falling of a neighbour domino can influence a given domino. Also, all dominoes fall at the same rate (i.e. a tick to complete the fall).

## HOW TO USE IT

There are three parameters to setup your own experiment. They are as follows:
- _dominoes-count_ : controls how many dominoes to simulate. (in increments of 10)
- _starter-dominoes_ : controls the starting number of falling dominoes. (in increments of 1)
- _propagation_ : allows you to control the number of sub-pieces that fall. (either 4 or 8, where the former refers to the north, south, east and west sub-pieces)

Click the SETUP button to set up the dominoes as per the parameters.

Click the GO button to start the simulation. The simulation will run until there are no more active pieces left.

TIP: Kindly use a slower tick rate to be able to better observe the propagation.

## THINGS TO NOTICE

As we randomly assign the positioning of dominoes, you should see isolated groups of dominoes. Depending on your parameters, some dominoes end up falling, while some do not at all.

Depending on the propagation model chosen, the rate of dominoes falling per tick will vary, as the 8-way propagation will tend to affect more neighbour dominoes.

## THINGS TO TRY

For a more exciting scenario, always choose a healthy value for _dominoes-count_ (preferably in the 100s).

You may choose any of the possible values for _starter-dominoes_ , but start with a lower number (<= 3) to be able to easily track the initial propagation.

Consider running the same parameter set multiple times as each iteration should have varying results, especially at lower _dominoes-count_ values.

## EXTENDING THE MODEL

This model can be enhanced by creating more sophisticated ways of arranging the dominoes, such as by controlling the amount of isolated groups.

Further work can be done in making the dominoes behave like the regular ones, by determining the larger faces of the dominoes, and consequently the direction of its fall.

Aesthetically, creating domino-specific shapes will also help!

## NETLOGO FEATURES

This is a fairly simple model, which manages to use advanced features NetLogo offers. Specifically the `neighbors(4)` primitive, which is used to perform the propagation of falling dominoes.

The above feature is specifically why only patches are used for representing the dominoes, however the more sophisticated models can consider using turtles with properties.

Otherwise, we also make use of major interface features offered by the program, especially monitors and plots for tracking the different states of dominoes throughout the simulation.

## RELATED MODELS

NetLogo Fire model

## CREDITS AND REFERENCES

* Wilensky, U. (1997).  NetLogo Fire model.  http://ccl.northwestern.edu/netlogo/models/Fire  Center for Connected Learning and Computer-Based Modeling, Northwestern University, Evanston, IL.

## HOW TO CITE

If you mention this model, kindly include the citations below.

* adbcode (2023).  Special Dominoes model.  https://github.com/adbcode/special-dominoes-model.  Data ScienceTech Institute, Biot, FR.

## COPYRIGHT AND LICENSE

Copyright 2023 adbcode.

This work is licensed under the MIT license. Please find the license attached in the source page linked in the citation above.
