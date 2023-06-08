# S110D-tof

This repository contains the ROS package for S100D and S110D Time-of-Flight (ToF) cameras.

## Installation

### Prerequisites

- ROS Noetic
- Ubuntu 20.04

### Steps

1. Install ROS Noetic and Ubuntu 20.04.
2. Clone this repository into the 'src' folder of your ROS workspace.
3. Open a terminal in your ROS workspace folder and execute the following commands:
```bash
catkin_make
catkin_make clean
```
Once the commands complete successfully, the ROS package for S100D or S110D should be installed.

## Usage

Follow the steps below to use the ROS package with the ToF cameras:

1. Start the ros master by running the following command in a terminal:
```bash
roscore
```
2. Open a new terminal and navigate to your ROS workspace folder. Source the ROS setup.
3. Plug-in the camera to the PC and verify its connection by running:
```bash
lsusb
```
You should see the camera listed.

4. Launch the ToF camera driver and nodes using the following command:
```bash
roslaunch cubeeye_scube depth_camera.launch
```
5. Open another terminal, source the ROS setup, and run RViz:
```bash
rosrun rviz rviz
```
6. In RViz, add the relevant topics and visualize the camera data.

Make sure to adjust the commands and instructions based on your specific ROS workspace and setup.


## License

This project is licensed under the MIT License.
