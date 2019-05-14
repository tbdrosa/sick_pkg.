# sick_pkg


# Introduction

This is meant to be run on terminal
/rosdistro: jade 
/rosversion: 1.11.21 
/RVis version: 1.11.18 (jade)

This is an introduction to using a SICK laser scanner connected to a ROS system. After reading this, you should be able to bring up the sicklms node and display the laser data. 

Make sure you have 

This is a pacakge to run for ROS IGVC to be used on SQRL. This pacakge uses sichtoolbox_wrapper and rvis to dispay point cloud data from the lidar.

# Installation

Instal sick toolbox using rosdep or other.

Then run <"rosmake sicktoolbox_wrapper rviz">

 # Hardware

- You will need a SICK LMS_291 LIDAR and a 24 V battery and a means to connect. 
- Once install is complete plug into the abttery and into the computer and check if it appears in the USB port. This should appear as "/dev/ttyUSB0". 

# Test it
- Open terminal
- In terminal type <"roscore">
- In a new terminal navigate to catkin_ws/src folder and install <sick_pkg> here
- after installing <sick_pkg> make sure <sick.launch> has proper access (if not then type <'chmod +x sick.launch'> ) 
- after launching make sure the phrase <sick.launch> text is green. Next, type into terminal <roslaunch sick.launch>
- You should now see sick.rvis grey 3D platform appear.
