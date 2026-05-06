BCR BOT - RUN COMMANDS :

===============================
Terminal 1 - Gazebo
===============================
cd ~/bcr_bot_ws
source /opt/ros/humble/setup.bash
colcon build --packages-select bcr_bot
source install/setup.bash
ros2 launch bcr_bot gazebo.launch.py


=====================================
Terminal 2 - Control (Keyboard)
=====================================
cd ~/bcr_bot_ws
source install/setup.bash
ros2 run teleop_twist_keyboard teleop_twist_keyboard


=====================================
Terminal 3 - RVIZ 
=====================================
cd ~/bcr_bot_ws
source install/setup.bash
ros2 launch bcr_bot rviz.launch.py


=====================================
Terminal 4 - Mapping (SLAM)
=====================================
cd ~/bcr_bot_ws
source install/setup.bash
ros2 launch bcr_bot mapping.launch.py


=====================================
Terminal 5 - Navigation (Nav2)
=====================================
cd ~/bcr_bot_ws
source install/setup.bash
ros2 launch bcr_bot nav2.launch.py
