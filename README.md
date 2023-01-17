# Non-linear-Control-of-RRbot-arm-in-MATLAB-and-Gazebo
## Overview
In this project, varous controllers for the control of RRbot arm are designed in MATLAB and simulated in Gazebo. This includes:
1. **State-feedback controller**: For bringing back the RRbot arm back to its initial position when disturbed.
2. **Feedback Linearization controller** (inverse dynamics controller): For tracking a quintic polynomial trajectory generated between start and end joint positions.
3. **Robust controller** (inverse dynamics robust controller): For tracking a quintic polynomial trajectory generated between start and end joint positions under uncertainities of the system.

The initial and final conditions for trajectory generation are: &theta;<sub>1</sub>(t<sub>0</sub>) = 180<sup>&deg;</sup>, &theta;<sub>1</sub>(t<sub>f</sub>) = 0<sup>&deg;</sup>, &theta;<sub>2</sub>(t<sub>0</sub>) = 90<sup>&deg;</sup>, &theta;<sub>2</sub>(t<sub>f</sub>) = 0<sup>&deg;</sup>, &theta;&prime;<sub>1</sub>(t<sub>0</sub>) =  &theta;&prime;<sub>1</sub>(t<sub>f</sub>) =  &theta;&prime;<sub>2</sub>(t<sub>0</sub>) =  &theta;&prime;<sub>2</sub>(t<sub>f</sub>) = 0<sup>&deg;</sup>. 

The output folder contains plots of the states(position and velocity) and torques of RRbot arm for each of the controller mentioned above. Plots from both MATLAB simulation and Gazebo simulation are presented. It is observed that for trajectory control Robust controller
is the better choice, since it works in a practical situation where we never know system parameters with 100% certainity. The chattering issue, wherein the torque fluctuates at high frequency between large values, is solved by incorporating boundary layer. The plots, with boundary layer and without boundary layer are presented.  
