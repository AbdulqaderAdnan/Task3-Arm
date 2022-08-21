AI-Task3-arm
-------------------------------------------------------------
after installing ROS successfully next is installing the arm package. Following the instruction in this link.

https://s-m.com.sa/ros.txt 
and changing the version form kinetic to noetic

Starting from this step "mkdir -p ~/catkin_ws/src"

The steps; 
----------------------------------------------
mkdir -p ~/catkin_ws/src

cd ~/catkin_ws/

catkin_make

cd ~/catkin_ws/src

git clone https://github.com/smart-methods/arduino_robot_arm.git

cd ~/catkin_ws

rosdep install --from-paths src --ignore-src -r -y

sudo apt-get install ros-noetic-moveit

sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui

sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher

sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control

sudo nano ~/.bashrc

at the end of the (bashrc) file add the follwing line (source /home/walaa/catkin_ws/devel/setup.bash) then ctrl + o

source ~/.bashrc

roslaunch robot_arm_pkg check_motors.launch

![لقطة الشاشة 2022-08-01 014822](https://user-images.githubusercontent.com/111324721/185774122-be1b9af0-af23-4999-b18d-bd0a39d2190b.jpg)


![arm](https://user-images.githubusercontent.com/111324721/185774132-fe4ceac8-9866-4a22-9cb6-e0b1826c4566.png)


