cmake_minimum_required(VERSION 2.8.3)
project(convert_to_csr)

find_package(catkin REQUIRED
  cmake_modules
)
find_package(Eigen REQUIRED)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  std_msgs
  moveit_commander moveit_core
  moveit_fake_controller_manager
  moveit_msgs
  moveit_planners_ompl
  moveit_ros_benchmarks
  moveit_ros_benchmarks_gui
  moveit_ros_control_interface
  moveit_ros_manipulation
  moveit_ros_move_group
  moveit_ros_perception
  moveit_ros_planning
  moveit_ros_planning_interface
  moveit_ros_robot_interaction
  moveit_ros_visualization
  moveit_ros_warehouse
  moveit_setup_assistant
  moveit_simple_controller_manager
  trajectory_msgs
  visualization_msgs
  rqt_moveit
  geometry_msgs
  eigen_conversions
  rosbag
  roslib
  tf
  tf_conversions
  pluginlib
  moveit_core
  geometric_shapes
  serial
)

catkin_package(
  
)

add_executable(ros_to_csr
  src/csr.cpp
)
add_dependencies(ros_to_csr ${${PROJECT_NAME}_EXPORTED_TARGETS} ${catkin_EXPORTED_TARGETS})
target_link_libraries(ros_to_csr
  ${catkin_LIBRARIES}
)

find_package(Eigen REQUIRED)

include_directories(
  include ${catkin_INCLUDE_DIRS}SYSTEM ${Boost_INCLUDE_DIR} ${EIGEN_INCLUDE_DIRS})

