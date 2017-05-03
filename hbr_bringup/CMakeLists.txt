cmake_minimum_required(VERSION 2.8.3)
project(hbr_bringup)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
)

catkin_package(
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)


install(FILES
  launch/bringup.launch
  launch/bringup_isolated.launch
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch
)
