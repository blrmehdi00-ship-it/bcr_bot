BCR BOT -  (ROS 2 HUMBLE)
Dependencies Installation:

sudo apt update
sudo apt install ros-humble-joint-state-publisher-gui ros-humble-xacro ros-humble-nav2-bringup ros-humble-slam-toolbox

Build and Run:

cd ~/bcr_bot_ws
colcon build --packages-select bcr_bot
source install/setup.bash

Execution Steps:

Terminal 1: Gazebo Simulation
source install/setup.bash
ros2 launch bcr_bot gz.launch.py

Terminal 2: Rviz Visualization
source install/setup.bash
ros2 launch bcr_bot rviz.launch.py

Terminal 3: Keyboard Control
source install/setup.bash
ros2 run teleop_twist_keyboard teleop_twist_keyboard

Terminal 4: SLAM (Mapping)
source install/setup.bash
ros2 launch bcr_bot mapping.launch.py

Terminal 5: Navigation (Nav2)
source install/setup.bash
ros2 launch bcr_bot nav2.launch.py

=====================================================
