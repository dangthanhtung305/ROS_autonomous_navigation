# AUTONOMOUS NAVIGATION OF MOBILE ROBOT USING KINECT SENSOR

## Overview
Design a mobile robot that can build a 2D map of an indoor environment (using SLAM system) and navigate from the robot's location to a point on the map.
The mobile base is a differential drive model. The robot software based on ROS (Robot Operating System) framework.

<p align="center">
  <img width="240" height="360" src="https://github.com/dangthanhtung305/ROS_autonomous_navigation/blob/master/image/mobile_base.png">
</p>

## Design system
- Use camera Kinect to collect environmental data (depth image), then convert depth image to laser scan and use it to build the 2D map
- Use Adaptive Monte Carlo Localization (AMCL) for localizing a robot's pose
- Do path planner to navigate the robot
- The robot uses PID controller and can calculate pose over time

Process data and build map:
<p align="center">
  <img width="700" height="200" src="https://github.com/dangthanhtung305/ROS_autonomous_navigation/blob/master/image/gmapping.png">
</p>


System diagram:
<p align="center">
  <img width="700" height="360" src="https://github.com/dangthanhtung305/ROS_autonomous_navigation/blob/master/image/system_flow.png">
</p>



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
Navigation based on the map build before
<p align="center">
  <img width="700" height="600" src="https://github.com/dangthanhtung305/ROS_autonomous_navigation/blob/master/image/robot_moving.png">
</p>

Avoid obstacles
<p align="center">
  <img width="700" height="600" src="https://github.com/dangthanhtung305/ROS_autonomous_navigation/blob/master/image/detect_obstacles.png">
</p>

## Youtube:
  - Mapping:  [here](https://www.youtube.com/watch?v=xC-JHz4ku9k)
  - Navigation: [here](https://www.youtube.com/watch?v=r-miZsWEDVE)
  - Navigation with obstacles: [here](https://www.youtube.com/watch?v=iaPCsaRBXBQ)


