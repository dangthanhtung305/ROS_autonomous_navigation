# AUTONOMOUS NAVIGATION OF MOBILE ROBOT USING KINECT SENSOR

## Overview
Design a mobile robot that can build a 2D map of an indoor environment (using SLAM system) and navigate from the robot's location to a point on the map
The mobile base is a Differential Drive model. The robot software based on ROS (Robot Operating System) framework

## Design system
- Use camera Kinect to collect environmental data (depth image), then convert depth image to laser scan and use it to build the 2D map
- Use Adaptive Monte Carlo Localization (AMCL) for localizing a robot's pose
- Do path planner to navigate the robot
- The robot uses PID controller and can calculate pose over time
## Dependencies
- Ubuntu 16.04
- ROS Kinetic Kam
- OpenNI 
- ROS packages:
  - depthimage_to_laserscan
  - gmapping
  - map_server
  - move_base
  - amcl
  - dwa_local_planner
## Result
