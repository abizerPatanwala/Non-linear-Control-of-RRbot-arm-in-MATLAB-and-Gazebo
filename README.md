# Non-linear-Control-of-RRbot-arm-in-MATLAB-and-Gazebo
##Overview
In this project, varous controllers for the control of RRbot arm are designed in MATLAB and simulated in Gazebo. This includes:
1. State-feedback controller: For bringing back the RRbot arm back to its initial position when disturbed.
2. Feedback Linearization controller: For tracking a quintic polynomial trajectory generated between start and end joint positions.
3. Robust controller: For tracking a quintic polynomial trajectory generated between start and end joint positions under uncertainities of the system.

The initial and final consitions for trajectory generation are: &theta;<sub>1</sub>(t0) = 180<sup>&deg;</sup>
