# ecse373_f23_hxp308_navvis_description
# Laboratory #2
## ROS Description of robots
1. URDF 
2. XACRO 
## Other used utilities in ROS 
1. ROS Neotic
2. ROS joint-state-publisher-gui
3. gazebo-plugins
4. ROS velodyne-description
## Commands for building & viewing robot
### Add the URDF for the robot to default /robot_description location
`rosparam set /robot_description -t <filename>.urdf`

### Run RVIZ with the saved configuration file (run from package root)
`rosrun rviz rviz -d config/config.rviz`

### Make a copy of the existing URDF file
> roscd <package_name>/urdf
> cp <filename>.urdf <filename>.xacro

### Set the /robot_description parameter from XACRO output
> rosparam set /robot_description "'rosrun xacro xacro filename.xacro'"


