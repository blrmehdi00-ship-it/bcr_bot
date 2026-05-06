*BCR Bot - ROS2 Simulation

This project is a ROS2 simulation of a mobile robot (BCR Bot) using Gazebo and RViz.
It allows manual control and autonomous navigation using Nav2.



* Requirements

- ROS2 (Humble / Jazzy)
- Gazebo
- RViz2
- colcon
- rosd


Controls:

- W → forward
- S → backward
- A / D → turn



* Features

- Mobile robot simulation
- Keyboard control
- Autonomous navigation (Nav2)
- Works with Gazebo and RViz
launch guide :


BCR BOT - RUN COMMANDS
=====================================

Terminal 1: Gazebo Simulation
-----------------------------
cd ~/bcr_bot_ws
colcon build --packages-select bcr_bot
source install/setup.bash
ros2 launch bcr_bot gz.launch.py

Terminal 2: Rviz Visualization
------------------------------
source install/setup.bash
ros2 launch bcr_bot visualize.launch.py

Terminal 3: Keyboard Control
----------------------------
source install/setup.bash
ros2 run teleop_twist_keyboard teleop_twist_keyboard

Terminal 4: SLAM (Mapping)
--------------------------
source install/setup.bash
ros2 launch bcr_bot slam.launch.py

Terminal 5: Navigation (Nav2)
-----------------------------
source install/setup.bash
ros2 launch bcr_bot navigation.launch.py


GitHub: blrmehdi00-ship-it 
