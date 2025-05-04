# Rosbot

## Overview

This repository provides a comprehensive template for quickly setting up a robotic application using ROS2. It includes the necessary configurations, files, and instructions to launch robot simulations, visualize robot states, and integrate control interfaces seamlessly.

## Features

* **Simulation:** Ready-to-use Gazebo simulation launch files.
* **Robot State Publisher:** Configuration and launch files for broadcasting robot states.
* **RViz Visualization:** Pre-configured RViz settings for robot model visualization.
* **Modular Structure:** Clearly organized directories for configurations, launch files, and robot descriptions.
* **ROS2 Control Integration:** Full support for ROS2 control interfaces.

## Getting Started

### Installation

1. Clone the repository:

```bash
git clone https://github.com/VaradHere/rosbot.git
cd rosbot
```

2. Install Dependencies:

Make sure your ROS2 environment is properly set up. Install any required dependencies (e.g., Gazebo, ROS2 Control) if not already installed.

```bash
sudo apt install ros-<ros2-distro>-gazebo-ros-pkgs ros-<ros2-distro>-ros2-control ros-<ros2-distro>-ros2-controllers
```

Replace `<ros2-distro>` with your installed ROS2 distribution (e.g., `humble`, `iron`).

### Running the Simulation

**Launch Gazebo Simulation:**

```bash
ros2 launch rosbot gazebo_sim.launch.py
```

**Visualize Robot in RViz:**

```bash
ros2 launch rosbot rsp.launch.py
```

## Directory Structure

```
rosbot/
├── config/             # Configuration files for RViz and controllers
├── launch/             # Launch files for simulation and robot state publisher
├── description/        # URDF and Xacro files defining the robot model
└── README.md           # Project documentation
```

## Contributing

Contributions are highly encouraged! To contribute:

1. Fork this repository.
2. Create a new feature branch (`git checkout -b feature/YourFeature`).
3. Commit your enhancements (`git commit -m "Add YourFeature"`).
4. Push the branch (`git push origin feature/YourFeature`).
5. Open a Pull Request.

## License

This project is licensed under the **Apache License 2.0**. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

This repository leverages a robust template designed for rapid ROS2 robotic application development. Special thanks to the open-source robotics community and all contributors.
