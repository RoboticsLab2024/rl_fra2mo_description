# Robotics Lab Mobile Robot

This repo provides URDF files and launch files to simulate a differential drive robot

```bash
colcon build --packages-select rl_fra2mo_description
. install/setup.bash
  ``` 
## Visualize on Rviz
```bash
ros2 launch rl_fra2mo_description display_fra2mo.launch.py
  ```
  
## Visualize on Rviz
```bash
ros2 launch rl_fra2mo_description gazebo_fra2mo.launch.py
  ```
  
## Send velocity command
```bash
ros2 topic pub /cmd_vel geometry_msgs/msg/Twist "{linear: {x: 0.2}, angular: {z: 0.2}}"
  ```
