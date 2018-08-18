# ROS File Server

A detached fork of [ROS# File Server](https://github.com/siemens/ros-sharp/tree/master/ROS/file_server) to keep deployments simple and reduce dependencies if the full ROS# package is not needed.

## Installation

Within your catkin workspace, clone this repository:

    cd ~/catkin_ws/src
    git clone https://github.com/gramaziokohler/ros_file_server.git

Install all dependencies:

    rosdep install -y --from-paths . --ignore-src --rosdistro kinetic

And build with `catkin build`:

    cd ~/catkin_ws
    catkin build

Or `catkin_make` if that's your thing:

    cd ~/catkin_ws
    catkin_make

Finally, source your catkin workspace:

    source ~/catkin_ws/devel/setup.bash

## Getting started

Once configured, starting the file server is simple:

    roslaunch file_server file_server.launch

## License

This project is a derivative work of the [ROS# File server](https://github.com/siemens/ros-sharp) and is open source under the same Apache 2.0 license as its original implementation.

## Credit

The original implementation of this project is copyrighted by Siemens AG, 2017 and was authored by [Dr. Martin Bischoff](https://github.com/MartinBischoff) (martin.bischoff@siemens.com).
