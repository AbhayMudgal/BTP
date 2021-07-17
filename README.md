# Dislocation Motion in the Presence of Diffusing Solutes: A Computer Simulation
The movement of dislocations dictates the deformative behavior of a material which has been extensively studied by Material Scientists for the practical applications of the materials. The interaction of dislocations with crystal defects play a key role in defining the deformation of a crystal. For example, the addition of little quantities of C to Fe produces steel which has significantly better physical properties compared to pure iron. The main component of the interaction is the interaction between the stress fields that these defects generate.  Analysis of related phenomena suggests that at lower driving forces the dislocations are pinned by solute atoms but at higher driving forces the motion is unimpeded by the solute atoms. The phenomenon at higher temperatures is dictated by the solute-dislocation interaction that depends on the dislocation velocity which in turn depends on the distribution of solute in the matrix. 

Kinetic Monte Carlo Methods have been extensively used to simulate the behavior of dislocations in various settings and a similar KMC model is used to study the behavior of dislocations in the presence of Cottrell atmospheres. The Monte Carlo model allows for stochastic solute diffusion, the formation of a solute cloud around the dislocation core and the motion of the Cottrell Atmosphere. The model considers the solute atoms to be misfitting spheres in an infinite isotropic linear elastic medium. The statistical mechanics of the solute distribution follows Fermi Dirac statistics and the solute concentration at a point does not exceed unity or that no two solute atoms may occupy one site due to quantum probabilities. 

The solute atoms are free to diffuse along the two dimensional solvent medium and at low driving forces form a protective barrier around the dislocation core inhibiting motion. In this study, the diffusing solute atoms interact with the edge dislocation gliding in either a positive or negative x-direction in two spatial dimensions. The Monte Carlo model is to show the behavior of solute atoms at high driving forces and the supposed retardation of the motion of the dislocation due to the interactions with the solute atoms.  

## Kinetic Monte Carlo Simulations
Macroscopic properties are the measurable properties of the system at the bulk level, e.g., the measured temperature, pressure and volume of the system. Following the principles of Statistical Mechanics, these macroscopic properties of the system can be generated as a summation of the microscopic properties. Any system undergoing a process goes through an infinite number of microstates. A Monte Carlo or the Molecular Dynamics simulation tries to replicate the same trajectory of the system by simulating a few of these microstates at discrete time intervals.

Several rules are defined to limit the scope of a simulation to generate plausible replicable models. The Monte Carlo simulation does not take into account the order in which the microstates are accessed, it only considers the list of microstates accessed and the frequency with which they were accessed. Another key feature of a Montecarlo Simulation is the dependence of the features being determined on the location. In MC simulations, the macroscopic property is only a function of the location or potential energy of the system and the kinetic energy is considered to be constant. 

Monte Carlo simulation consists of three steps:
1. Sampling
2. Evaluation
3. Decision
Steps 1, 2 and 3 define an iteration of the Monte-Carlo algorithm which is called a “trial”.

## Simulation Method
The model assumes that there is minimal interaction between the solute atoms and that can be neglected. The only interaction that is responsible for change in energy of the system is that of the solute atom and the single dislocation. The solute atoms are strictly substitutional. Both the solute atoms and the dislocation are constrained to move on the sites of the square lattice and each movement in a trial is of the magnitude of one burgers vector b, which is assumed to be 1 to simplify the process. Initially the dislocation is placed at the center of the two-dimensional simulation cell and the solute atoms are distributed randomly throughout the cell subject to Fermi Dirac Statistics. 

The simulation is run with the parameters presented in the code. These can be varied to suit differnt settings in industrial applications. The code is generic and can be modified to suit variety of systems by inputing the parameters at the beginning instead of assuming hard coded values that are used in the models. 
- BTP_v2 represents the case where the dislocation is static and only the solute atoms diffuse
- BTP_v3 represents the case of a dynamic dislocation and solute atom
- BTP_v4 represents the case in which mulitple solute atoms are present and a static dislocation.
