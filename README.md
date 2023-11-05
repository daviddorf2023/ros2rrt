# RRT_2D_3D


https://github.com/daviddorf2023/ros2rrt/assets/113081373/681f2f3d-e7b1-4488-a605-03b472c3581f


https://github.com/daviddorf2023/ros2rrt/assets/113081373/dd4268d0-8ca6-4d42-8f72-c304640ba5f7

## Description
3D and 2D implementation of Rapid Exploring Random Tree algorithms for ROS 2. The main ROS 2 nodes are rrt2D and rrt3D, which can take user inputs and publish the nodes of the RRT and the path to the goal. The ROS 2 nodes are currently in development. The nodes can subscribe to topics for map data, marker obstacles, and can be launched with rrt2Dlaunch.xml and rrt3Dlaunch.xml, respectively.

## Installation
### Dependencies
* ROS 2 Iron
* Python 3.5+
* numpy 1.13.3+
### Building
Clone the repository into your ROS 2 workspace and build with colcon build.

## Usage
### ROS 2 Nodes
#### rrt2D
rrt2D is a ROS 2 node that implements the RRT algorithm in 2D. It can be launched with the rrt2Dlaunch.xml file. The node subscribes to the /occupancy_grid topic for map data and the /obstacle_markers_2D topic for marker obstacles. The node publishes the nodes of the RRT to the /rrt_markers topic and the path to the goal to the /rrt_path topic.
#### rrt3D
rrt3D is a ROS 2 node that implements the RRT algorithm in 3D. It can be launched with the rrt3Dlaunch.xml file. The node subscribes to the /occupancy_grid topic for map data and the /obstacle_markers_3D topic for marker obstacles. The node publishes the nodes of the RRT to the /rrt_markers topic and the path to the goal to the /rrt_path topic.

## Authors and Contributors
Author: David Dorf
