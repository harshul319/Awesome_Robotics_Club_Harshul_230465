# Awesome_Robotics_Club_Harshul_230465
Summer robotics task-

Robotic Arm-

Base configeration of robot is set so that the position of joints are as follows-

base joint (can rotate about z)-(0,0,0)

joint0 (can rotate about y)-(0,0,23)

joint1 (can rotate about y)-(15,0,23)

joint2/endeffector -(20,0,23)

So the code basically use change of axis for the position of the object to project it in the x-z plane while measuring the angle that should be rotated by base angle to attain the situation and applies FABRIK algorithm to configure the positions of joint 0 and 1 in 2D space of x and z and the angles are configured by applying cosine formula 

Some shortcomings of the code-

1. Was not able to put angle constraints for the reachability of the arm 
2. Some special configerations of the arm are glitching for eg theta 2 angle is coming to be -90 degrees in both position of object (0,15,28) and (0,15,18)(whereas it should show +90 for (0,15,18)



Some examples of code working with different positions of object are given in the python notebook-![Screenshot (3)](https://github.com/harshul319/Awesome_Robotics_Club_Harshul_230465/assets/153108163/74c6dd4f-01fa-453d-83a8-26d901594496)


