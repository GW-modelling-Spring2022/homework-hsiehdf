# The Discussion
### 1 Does the equipotential distribution depend on the absolute or relative K values for the background and the inclusion? How would you use the model to test your answer?
* I think the equipotential distribution would depend on the relative K values for both the background and the inclusion. Keq is calculated using the harmonic average and it wouldn't make sense that the equipotential distribution would depend on the arithmetic mean because it isn't used. 
* To test this I would plot the contour head plots of both scenarios using Keq vs arithmetic K and see whether the head plot made sense. 
### 2 Discuss what it means to say that, for steady state flow, there are equivalent Type I and Type II boundary conditions. How might this be useful in practice?
* When we have steady state flow there is no change in storage and therefore flux is constant everywhere. Type 1 conditions are constant head and type 2 conditions are constant flux. In steady state we can have the same model using either Type 1 or Type 2 boundary conditions. 
*  For instance, if we have a constant head value that gives us a Hydraulic head gradient of 5 and a hydraulic conductivity value of 2,  we can create the exact same scenario using a constant flux of 10 (given the same K)

### 3 What would you find if you altered your model to consider unconfined conditions??
* The head profile would no longer be linear. This has something to do with the cross sectional area not being constant... but I need more discussion about this to understand it better.

# Glossary Questions
### 1. What is FloPy? How is it different from MODFLOW and how does it interact with MODFLOW? What are some advantages (easy) and disadvantages (harder) of using FloPy rather than building MODFLOW models manually?
* Flopy runs MODFLOW through python. Code is written that generates and sends text files that MODFLOW needs in order to produce its outputs. These outputs are then read in Flopy and analysis can be conducted on the outputs using python code. 
* Advantages- large data sets can be analysed 
* Disadvantages- You need to know how to use python/code 
### 2. Given that the distribution of K is always heterogeneous at the small scale, what does it mean to provide one K value per grid cell? What are the implications for the K values we use in models in general? How does this change if we are modeling with different spatial resolutions (i.e. grid cell sizes)?
* We are assuming each grid is a REV (representative elemental volume), even when it isn't. If we want better resolution we need smaller grid sizes.
  
### 3. What does it mean for a groundwater model to be confined? How does this simplify calculations of groundwater flux? How do we specify this with cell types in MODFLOW?
* A confined GW model means that there are boundaries that are either not active or impermeable. This would restrict flow to those places. If we have a steady state model our head profile will always be linear. We change the .bas file from 0, 1, or -1