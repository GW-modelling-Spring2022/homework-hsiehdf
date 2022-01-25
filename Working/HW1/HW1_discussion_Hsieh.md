# Assignment
What are boundary conditions? Answer this both conceptually and mathematically.
    Constant Head boundary on the top and bottom. The top head is 100 and the bottom is 0. 
What are model parameters? How do they (and don't they) represent the actual subsurface?
    
What are steady state conditions and how can they be identified from the Excel model results?
    Steady State means that storage in our system (control volume) is equal to zero, which consequently means that our input is equal to our output. We can see we have steady state conditions because our flux is constant
Can you imagine how the model inputs could be stored in separate files rather than other spreadsheet cells? Describe the flow of information from a file that describes the other files that contain model-specific information about the system.
    We could have seperate files that would calculate different parameters of our model. Then we would have one file that would call our other files and sythesize our data using specific paramters??
What is an iterative solution? Can you explain it to a hydrologist who is not a modeler? Can you describe (or imagine) how Excel finds the solution?
    An iterative solution is one that uses a previous solution to calculate a subsequent solution. 
What is a direct solution? What are its (dis)advantages compared to an iterative (numerical) solution?
    A direct solution can be thought of as a process where our inputs do not change in our problem. Therefore the answer will always be the same given the same inputs. It is quicker but less accurate than an iterative solution.