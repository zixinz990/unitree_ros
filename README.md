# unitree_ros

This repository is a fork of [unitreerobotics/unitree_ros](https://github.com/unitreerobotics/unitree_ros) and serves for [RoboticExplorationLab/legged_mpc_control](https://github.com/RoboticExplorationLab/legged_mpc_control). It will be automatically installed when you install legged_mpc_control.

The main differences between this repository and the original `unitree_ros` are:

1. Deleted files about z1.
2. Modified unitree_move_kinetic. When the user run `rosrun unitree_controller unitree_move_kinetic`, the robot will be fixed in a default pose instead of rotating around the Z-axis.
3. Modified ODE parameters in Gazebo world files. Contact simulation becomes more accurate.
4. Modified Gazebo plugins in A1 and Go1 models. `libLinkPlot3DPlugin` is removed. `libgazebo_ros_p3d` is added to get the ground truth of torso's pose.
5. `unitree_legged_msgs` and `unitree_legged_real` are included in this repository.