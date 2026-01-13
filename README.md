# ROS2 examples

This repo contains ROS2 (jazzy) examples from https://github.com/ros2/examples/tree/jazzy.
A top-level CMakeLists.txt is provided that allows opening the examples in CLion, 
which adds code-completion and insights for both the Python and C++ source. 
To make Python work, you need to assign an interpreter. On Windows you should use the one that comes with ROS2 (`C:\pixi_ws\.pixi\envs\default\python.exe`).

A `colcon_build` target is also added, which may be used to build the ROS2 packages.

## Running the examples

> Start by building the workspace with colcon (see above). Do this each time you make changes to the workspace.

In one terminal run:
`ros2 run examples_rclcpp_minimal_publisher publisher_member_function`

In another terminal run:
`ros2 run examples_rclcpp_minimal_subscriber subscriber_member_function`

In each terminal you must first run `./install/setup.*` (.bash on linux, .bat in cmd and .ps1 in PowerShell) to source the workspace.
