# Awesome_Robotics_Club_Harshul_230465
Summer robotics task

 Bandit over the wire-
 Level 1- ls to veiw folders in the directory and cat readme to access the file readme
 
 Level 2- ls to veiw folders in the directory and cat <- to access the file - (< or ./ should be used to read files initiated with -)
 
 Level 3- ls to veiw folders in the directory and cat "spaces in this filename" to access the file 'spaces in this filename'(so it reads whole as a single string)
 
 Level 4- ls to veiw -> we get inhere directory -> cd to get into inhere -> ls -a to show hidden files -> cat .hidden to veiw .hidden file
 
 Level 5- ls to veiw -> we get inhere directory -> cd to get into inhere -> ls to view -> find . -type f | xargs file to find files in all the directories and then also state the type of the file -> only file 7 has the human readable file which is the password
 
![image](https://github.com/harshul319/Awesome_Robotics_Club_Harshul_230465/assets/153108163/5dd0b70a-7800-4304-b5f0-7c58cdac9c66)


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


