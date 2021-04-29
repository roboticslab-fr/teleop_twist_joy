teleop_twist_joy [![Build Status](https://travis-ci.org/ros-teleop/teleop_twist_joy.svg?branch=indigo-devel)](https://travis-ci.org/ros-teleop/teleop_twist_joy)
================

Simple joystick teleop for twist robots. See [ROS Wiki](http://wiki.ros.org/teleop_twist_joy)

## For Logitech F710 Joystick :

### Hardware Settings
**!!! front switch on D !!!**

Dead man button = LB

More infos in the [Logitech F710 HowTo Memo](https://github.com/roboticslab-fr/teleop_twist_joy/blob/indigo-devel/documentation/Logitech-F710-Pad_HowTo.pdf)

### Launch joystick

    $ roslaunch teleop_twist_joy teleop.launch joy_config:="f710"
OR

    $ roslaunch teleop_twist_joy logitech.launch

### Useful command to DEBUG
    $ sudo chmod a+rw /dev/input/js0
    $ rosparam set joy_node/dev "/dev/input/js0"
