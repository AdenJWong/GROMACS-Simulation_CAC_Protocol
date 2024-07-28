# GROMACS_Simulation_CAC_Protocol

## Set up

To run Gromacs Molecular Dynamics simulations we will first need to set up our prerequisites and environments in the CAC Frontenac cluster (https://cac.queensu.ca/)

1. Access Cluster: <br/>
   CAC access can be requested using the following link: https://cac.queensu.ca/ <br/>
   Instructions on usage can be found https://login.cac.queensu.ca/basic-usage.shtml

2. Environment set up:
   Use the following command the request additional resources such as a gpu
   ```bash
   salloc --gres=gpu:1 -c 10 --mem 40g -t 8:0:0 #
   ```
   
   Use this command to list the modules avaiable for use
   ```bash
   module spider <name>
   ```
   
   In our case we will be loading the most recent version of Cuda available to us
   ```bash
   module load cuda/11.6.1
   ```
