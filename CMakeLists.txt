cmake_minimum_required(VERSION 3.5.1)

project(trikey_control)

find_package(catkin REQUIRED COMPONENTS
controller_manager
joint_state_controller
robot_state_publisher
)

catkin_package()

install(DIRECTORY config
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})

install(DIRECTORY launch
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})