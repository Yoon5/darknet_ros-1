YOLO for ROS on Jetson

This is darknet ROS for Nvidia Jetson.

# wait  for builiding
$ cd ~/catkin_ws/

$ catkin_make 

# memory, source setup.
$ cd ~/catkin_ws/

$ source ./devel/setup.bash

# All  seperate terminal
$ roscore

$ rosrun usb_cam usb_cam_node /usb_cam/image_raw:=/camera/image_raw

$ roslaunch darknet_ros darknet_ros.launch

$ rosrun rqt_graph rqt_graph
