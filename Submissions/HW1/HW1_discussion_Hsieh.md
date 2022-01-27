# Challenge Questions for HW1

### 1. Show, based on the flux with depth, that the model is steady state. Repeat this for a homogeneous and for a heterogeneous column.
- From the pdf there are two figures that contain a elevation vs flux figure. Both of these figures have a straight vertical line which shows that the model is in a steady state (because flux is not changing). 

### 2. Show that the steady state flux agrees with the direct calculation based on the harmonic mean average K. Write the equation defining the direct calculation of the flux.
* The direct calculation of flux is Darcy's Law: q = -K *(dH/dz)
* If we perform the direct calculation using our Keq (0.00025, calculated using the harmonic mean of the different K's) the answer is the same as that expressed in the excel

### 3. Show the steady state head profile for a column with approximately equal-thickness layers that have different K values.
* Refer to pdf

### 4. Use the head profile to explain WHY the equivalent hydraulic conductivity, Keq, is closer to the lower of the two K values.
* The lower the hydraulic conductivity, the more that the head drops over that respective area. This is because our system is in steady state, therefore, the flux is the same throughout our column. 
# Discussion for HW1

## 1. What are boundary conditions? Answer this both conceptually and mathematically.
* Boundary conditions are spatial conditions that the model is bound by. In the case of my excel it was a constant Head boundary on the top and bottom. The top head is 100 and the bottom is 0. 
## 2. What are model parameters? How do they (and don't they) represent the actual subsurface?
  * A model parameter is an input that is used to calculate another value. For our example model our parameter is hydraulic conductivity. Hydraulic conductivity is only an approximation of how fluid flows in the subsurface. It is not an exact representation of how fluids may flow in the subsurface. 
  
## 3. What are steady state conditions and how can they be identified from the Excel model results?

* Steady State means that storage in our system is equal to zero, which consequently means that our input is equal to our output. We can see we have steady state conditions because our flux is constant


## 4. Can you imagine how the model inputs could be stored in separate files rather than other spreadsheet cells? Describe the flow of information from a file that describes the other files that contain model-specific information about the system.
* We could have separate files that would each calculate different parameters of our model. Then we would have one file that would call all of our files at once and synthesize the data. 
  
## 5. What is an iterative solution? Can you explain it to a hydrologist who is not a modeler? Can you describe (or imagine) how Excel finds the solution?
* An iterative solution is one that uses a previous solution to calculate a subsequent solution. Excel will take a previous hydraulic head solution to calculate a subsequent flux value. The amount of iterations taken is something the modeler can specify.

## 6. What is a direct solution? What are its (dis)advantages compared to an iterative (numerical) solution?
 *  A direct solution is one where we have a set number of steps needed to reach a solution. All steps must be completed in order to reach a solution. A direct solution can be quicker to reach a solution, but it will likely not be as accurate as an iterative solution. 