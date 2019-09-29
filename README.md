# Steel 3D printing using Wire Arc Additive Manufacturing (WAAM) with an ABB IRB 1400

# Note
This module was written as part of my KPI's for Steelo LTD. 

# Requirements
1. ABB robot
2. Fronius tps 320i
3. Welding table
4. RobotStudio (Rapid Programming)

# Description
This repo contains rapid code to 3D print two basic geometric shapes: square and circle in steel. Users have to manually enter parameters to define the size of the shape like radius of the circle, and height and length for the square. 

Once the robot finishes moving through the defined path, the robot moves up by 3mm to repeat the movement. This change in z-axis is experimental which proved successful for building shapes with more than 5cm tall. Time was given for each layer to allow cooling and avoid accumulation of heat stress.

Only simple shapes could have printed as there was no access to any software that would convert a 3D model into a program that is readable to the ABB IRB 1400. Also, the in-house robot used an s4 controller which is not compatible with RobotStudio, therefore Notepad was used to rewrite some of the code that was developed in RobotStudio.
