# Lino Installation

The install file has been updated to enable 2wd/rplidar on ROS noetic. Other settings are not tested.

The `install` file will install all the files you need to build an autonomous robot including:
- Teensy Firmware
- Sensor Driver
- Navigation Stack

You need to pass two arguments to the install file, where:
```
$ ./install <base> <sensor>
```
Example
```
./install 2wd rplidar
```

##### base 
The type of robot you want to build. Valid arguments are 
- 2wd
- 4wd (not updated for noetic)
- ackermann (not updated for noetic)
- mecanum (not updated for noetic)

##### sensor 
The lidar you're going to use for your build. Valid arguments are 
- xv11 (not updated for noetic)
- rplidar
- ydlidar (not updated for noetic)
- hokuyo (not updated for noetic)
- kinect (not updated for noetic)
- realsense (not updated for noetic)

:exclamation: Do note that for hokuyo lidar, you will be prompted for the IP address (Default: 192.168.0.10)

## Installation Guide

* Clone the repo and `cd` into the folder

  ```
  git clone https://github.com/iangohy/lino_install.git
  cd lino_install
  ```

* Install

  ```
  ./install 2wd rplidar
  ```

  