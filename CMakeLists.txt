cmake_minimum_required(VERSION 2.8.3)
project(ros_erle_takeoff_land)

## Find catkin and any catkin packages
find_package(catkin REQUIRED COMPONENTS roscpp rospy std_msgs genmsg)

## Generate added messages and services
generate_messages(DEPENDENCIES std_msgs)

## Declare a catkin package
catkin_package()

include_directories(include ${catkin_INCLUDE_DIRS})

add_executable(ros_erle_takeoff_land src/main.cpp)
target_link_libraries(ros_erle_takeoff_land ${catkin_LIBRARIES})
add_dependencies(ros_erle_takeoff_land ros_erle_takeoff_land_generate_messages_cpp)

install(
	TARGETS ros_erle_takeoff_land
	ARCHIVE DESTINATION ${CATKIN_PACKAGE_LIB_DESTINATION}
	LIBRARY DESTINATION ${CATKIN_PACKAGE_LIB_DESTINATION}
	RUNTIME DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})
