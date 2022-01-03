# [[ROS] Controls](#ros-controls)

## [MoveIt!](#moveit)
MoveIt is a set of packages for your robot to manipulate for Motion Planning, Manipulation, Inverse Kinematics, Control, 3D Perception and Collision Checking. 

The following instruction describes how to install moveit package and to use MoveIt with OpenMAIPULATOR-P.

### [Install MoveIt Packages](#install-moveit-packages)

```bash
$ cd ~/catkin_ws/src/
$ git clone https://github.com/ROBOTIS-GIT/open_manipulator_p_controls.git
$ git clone https://github.com/ROBOTIS-GIT/open_manipulator_dependencies.git
$ cd ~/catkin_ws && catkin_make
```

### [Launch MoveIt!](#launch-moveit)
Run **Moveit!** with the following command.

  ``` bash
  $ roslaunch open_manipulator_p_controllers joint_trajectory_controller.launch sim:=false
  ```
  
  ![](/assets/images/platform/openmanipulator_p/moveit_launch.png)  
  
#### [Using MoveIt! with Gazebo](#using-moveit-with-gazebo)
Gazebo is a tool to simulate and test your robot in a virtual enviroment, without an actual robot.  

Also, you can use MoveIt feature using your virtual robot in the gazebo enviroment with the following command.

For more information on Gazebo, See [Simulation](/docs/en/platform/openmanipulator_p/ros_simulation/#ros-simulation)

```bash
$ roslaunch open_manipulator_p_controllers joint_trajectory_controller.launch
```
