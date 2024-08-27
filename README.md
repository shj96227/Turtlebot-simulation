# Turtlebot-simulation
간단한 터틀봇 시뮬레이션을 해보았다.

## Overview
![turtlebot](https://github.com/user-attachments/assets/a887df95-03bd-4e7c-b33a-3eed7e79390a)

## Getting Started
### 1. Clone


```sh
sudo apt-get install ros-melodic-joy ros-melodic-teleop-twist-joy \
  ros-melodic-teleop-twist-keyboard ros-melodic-laser-proc \
  ros-melodic-rgbd-launch ros-melodic-depthimage-to-laserscan \
  ros-melodic-rosserial-arduino ros-melodic-rosserial-python \
  ros-melodic-rosserial-server ros-melodic-rosserial-client \
  ros-melodic-rosserial-msgs ros-melodic-amcl ros-melodic-map-server \
  ros-melodic-move-base ros-melodic-urdf ros-melodic-xacro \
  ros-melodic-compressed-image-transport ros-melodic-rqt* \
  ros-melodic-gmapping ros-melodic-navigation ros-melodic-interactive-markers

cd ~/catkin_ws/src/
git clone -b melodic-devel https://github.com/ROBOTIS-GIT/turtlebot3.git

git clone -b melodic-devel https://github.com/ROBOTIS-GIT/turtlebot3_msgs.git

git clone -b melodic-devel https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git

cd ~/catkin_ws && catkin_make
```

### 2. Simulation with RViz

시뮬레이션 / RViz를 뷰어로 사용할 경우
```sh
export TURTLEBOT3_MODEL=burger
roslaunch turtlebot3_fake turtlebot3_fake.launch
```
w,a,s,d 를 사용하여 turtlebot 이동
```sh
export TURTLEBOT3_MODEL=burger
roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
```
