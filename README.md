*BCR Bot - ROS2 Simulation

This project is a ROS2 simulation of a mobile robot (BCR Bot) using Gazebo and RViz.
It allows manual control and autonomous navigation using Nav2.

---

* Requirements

- ROS2 (Humble / Jazzy)
- Gazebo
- RViz2
- colcon
- rosd

---

* Install dependencies

cd ~/ros2_ws
rosdep install --from-paths src --ignore-src -r -y

---

* Build the project

colcon build
source install/setup.bash

---

* Run the simulation

ros2 launch bcr_bot gazebo.launch.py

---

  * Manual control (Keyboard)

Open a new terminal:

cd ~/ros2_ws
source install/setup.bash
ros2 run teleop_twist_keyboard teleop_twist_keyboard

Controls:

- W → forward
- S → backward
- A / D → turn

---

 * Autonomous Navigation (Nav2)

Run navigation:

source install/setup.bash
ros2 launch nav2_bringup navigation_launch.py

Then open RViz and:

- Use "2D Goal Pose"
- Select a goal on the map
- Robot moves automatically

---

* Project Structure

- "launch/" → launch files
- "urdf/" → robot model
- "worlds/" → Gazebo world
- "config/" → navigation parameters

---

* Features

- Mobile robot simulation
- Keyboard control
- Autonomous navigation (Nav2)
- Works with Gazebo and RViz

---


GitHub: blrmehdi00-ship-it 
