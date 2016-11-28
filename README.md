This is a fork of the 2016 ACC Manuscript long version. 

https://github.com/skulumani/2016_acc_manuscript/tree/long_version

We're modifying/expanding it for submission to IJCAS

http://www.springer.com/engineering/robotics/journal/12555

## To regenerate the plots

The code used to generate these plots are the same as the 2016 ACC paper.

You can find the matlab code:

https://github.com/skulumani/2016_ACC_matlab

And the experimental data:
https://github.com/skulumani/2016_ACC_Experiment

Look at the README in each of those to regenerate the plots

## To regenerate the figures for publications

### Configuration Error Function visualization:
run log_barrier.m to make the surface plots for the \Psi

Go to commit a4e97e069d475b1760d61db2d46c1157281afe1c to make sure the constants
are setup properly

### Attitude Stabilization without adaptive update law:
run coupled_control_driver.m and then run plot_outputs.m to generate the simulation
plots used in both ACC/IJCAS submission

This is also using commit a4e97e069d475b1760d61db2d46c1157281afe1c

### Attitude Stabilization with adaptive update law:
run coupled_control_driver.m and then run plot_outputs.m or draw_cad to generate
the plots. There's a flag in load_constants to create animations or a video

Go to commit 6f5604a9db17ee67b019dac6daa1807e5ed3c6d5 to ensure the constants 
are setup properly

### Constrained Attitude stabilization experiment:
Run Data_analysis.m to read 20150924_avoid3.txt to generate the experimental results

The repository holding the experimental data is located at
https://github.com/skulumani/2016_ACC_Experiment

The commit is 6f5604a9db17ee67b019dac6daa1807e5ed3c6d5

This calls load_experiment_constants and plot_experiment_constants 