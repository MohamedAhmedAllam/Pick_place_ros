# Pick_place_ros
Pick and place - motion planning of a real 6-DOF manipulator using ROS  

Mechatronics course project  

For all project details read the file report.pdf

Project video: https://youtu.be/WUDkOi_OQT8

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


![alt text](https://github.com/MohamedAhmedAllam/Pick_place_ros/blob/master/photos/Gazebo_pick_book_arm.png)  

![alt text](https://github.com/MohamedAhmedAllam/Pick_place_ros/blob/master/photos/Our_arm_position(0.3%2C0.2%2C1.4).png)  

![alt text](https://github.com/MohamedAhmedAllam/Pick_place_ros/blob/master/photos/Our_arm_position(0.5%2C0.5%2C0.5).png)  

![alt text](https://github.com/MohamedAhmedAllam/Pick_place_ros/blob/master/photos/Rviz_pick_book_arm.png)  

![alt text](https://github.com/MohamedAhmedAllam/Pick_place_ros/blob/master/photos/Rviz_place_book_arm.png)  
