# CanadaArm2 ROS 2 Description Package

<div align="center">
  <img src="https://github.com/1412kauti/canadarm2_description/blob/main/assets/autodesk_fusion.png" width="32%" alt="Fusion 360 Model"/>
  <img src="https://github.com/1412kauti/canadarm2_description/blob/main/assets/isaac_sim.png" width="32%" alt="Isaac Sim Model"/>
  <img src="https://github.com/1412kauti/canadarm2_description/blob/main/assets/urdf_viz.png" width="32%" alt="urdf-viz Model"/>
</div>

## Overview

This repository contains the ROS 2 description package for the **CanadaArm2** robotic manipulator.
It provides the URDF, meshes, and launch files needed for visualization and simulation in ROS 2 environments such as RViz, Gazebo, Isaac Sim, and urdf-viz.

## Features

- Detailed URDF model with physical properties and joint limits
- High-quality mesh files (`.stl`/`.dae`/`.obj`/`.ply`) for simulation and visualization
- Ready-to-use launch files for RViz and Gazebo
- Compatible with ROS 2 Humble and Jazzy


## Quick Start
### Prerequisites
```bash
sudo apt install ros-jazzy-joint-state-publisher ros-jazzy-joint-state-publisher-gui ros-jazzy-robot-state-publisher ros-jazzy-rviz2 ros-jazzy-ros-gz -y
```
### 1. Clone and Build

```bash
cd ~/ros2_ws/src
git clone https://github.com/1412kauti/canadarm2_description.git
cd ~/ros2_ws
colcon build
source install/setup.bash
```


### 2.1 Visualize in RViz

```bash
ros2 launch canadarm2_description display.launch.py
```

### 2.2 Visualize in Gazebo

```bash
ros2 launch canadarm2_description gazebo.launch.py
```

## Usage in Other Simulators

- **Isaac Sim:** Import the URDF and meshes directly.
- **urdf-viz:**

```bash
urdf-viz urdf/canadarm2.urdf
```
## License

[MIT](LICENSE)

## Acknowledgments

- Original Files found [here](https://www.printables.com/model/235290-canada-arm-2)
- ROS 2 and open-source robotics community

**Happy simulating! 🤖**
