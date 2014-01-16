project(smach_viewer)
cmake_minimum_required(VERSION 2.8.3)

find_package(catkin REQUIRED)

catkin_package(
  CATKIN_DEPENDS smach_ros xdot smach_msgs
)

# Install targets
install(PROGRAMS scripts/smach_viewer.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})
