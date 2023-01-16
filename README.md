# Non-linear-Control-of-RRbot-arm-in-MATLAB-and-Gazebo
##Overview
In this project, varous controllers for the control of RRbot arm are designed in MATLAB and simulated in Gazebo. This includes:
1. State-feedback controller: For bringing back the RRbot arm back to its initial position when disturbed.
2. Feedback Linearization controller: For tracking a quintic polynomial trajectory generated between start and end joint positions.
3. Robust controller: For tracking a quintic polynomial trajectory generated between start and end joint positions under uncertainities of the system.

The initial and final consitions for trajectory generation are: &theta;<sub>1</sub>(t<sub>0</sub>) = 180<sup>&deg;</sup>, &theta;<sub>1</sub>(t<sub>f</sub>) = 0<sup>&deg;</sup>, &theta;<sub>2</sub>(t<sub>0</sub>) = 90<sup>&deg;</sup>, &theta;<sub>2</sub>(t<sub>f</sub>) = 0<sup>&deg;</sup>, &theta;&prime;<sub>1</sub>(t<sub>0</sub>) =  &theta;&prime;<sub>1</sub>(t<sub>f</sub>) =  &theta;&prime;<sub>2</sub>(t<sub>0</sub>) =  &theta;&prime;<sub>2</sub>(t<sub>f</sub>) = 0&deg; 
