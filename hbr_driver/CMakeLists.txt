cmake_minimum_required(VERSION 2.8.3)
project(hbr_driver)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  std_msgs
)

catkin_package(
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)

install(PROGRAMS
  scripts/driver.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
