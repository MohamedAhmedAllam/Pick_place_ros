# Pick_place_ros
Pick and place - motion planning of a 6-DOF manipulator


src folder for the whole workspace:
Downlaod src.zip, unzip in a folder then run catkin_make

Launch Gazebo for grasping:
$ roslaunch seven_dof_arm_gazebo seven_dof_arm_bringup_grasping.launch

Start MoveIt! motion planning:
$ roslaunch seven_dof_arm_config moveit_planning_execution.launch

Launch MoveIt! Grasp server:
$ roslaunch seven_dof_arm_gazebo grasp_generator_server

Run the Grasp client:
$ rosrun seven_dof_arm_gazebo pick_only.py

Run the place node
$ python "workspace_directory"/src/seven_dof_config/scripts/debug_code.py

Works only on ubuntu 14.04.02
Tested only on "mastering ros for robotics" arm
