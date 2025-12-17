## NavierStokes-Equation: simulating the Kármán vortex street (Kármánsche Wirbelstraße)

Collaborators:
- Emanuel Steininger
- Martin Strobl
- Anna Sonnleitner




## NG Solve documentation

# ChatGPT

first command for Copilot was straightforward:

    Hello, I have a task for you. Can you please create a code for a Jupyter notebook that simulates a flow using NGSolve? 
    To do this, it should solve the Navier-Stokes equations using the finite element method (FEM).
    The flow should be disturbed by a cylindrical obstacle, which the simulation should take into account and thus also depict the vortices generated after the obstacle. (Karman vortex street)
    Constant density and incompressibility can be assumed.

it worked fine but calculated the trivial solution of u=0

after demonstraiting this fact, it tried to solve this problem, by creating a stream, but then the preassure-function could not be calculated/drawn anymore

-> it changed Q from L2 to H1
still same problem

had a lot of problems, told him it should not work with the 'Oseen-Form', but with ... and use a little preassure-stabilisation: 
