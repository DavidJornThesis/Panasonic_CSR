# Panasonic_CSR

## Introduction

In this repository, a start has been made to make a conversion of ROS commands to a csr-file
which can be used in the DTPS software of Panasonic manipulators. In this repo, a Panasonic 
VR-006L manipulator is used.

## Installation

To install this repo, just clone it into your workspace:

cd ~/catkin_ws/src

git clone -b 'branch' 'github-webcode'

source devel/setup.bash

catkin_make


## Usage

After the installation, a launch can simply be launched as follows:

roslaunch convert_to_csr ros_to_csr.launch
