################################################################################
# Set minimum required version of cmake, project name and compile options
################################################################################
cmake_minimum_required(VERSION 2.8.3)
project(turtlebot3c_2dnav)

find_package(catkin REQUIRED)
catkin_package()

################################################################################
# Install
################################################################################

catkin_install_python(PROGRAMS scripts/mapping_manager
                      DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})

install(DIRECTORY launch
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
