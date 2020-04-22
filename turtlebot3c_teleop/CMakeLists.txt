################################################################################
# Set minimum required version of cmake, project name and compile options
################################################################################

cmake_minimum_required(VERSION 2.8.3)
project(turtlebot3c_teleop)

find_package(catkin REQUIRED)
catkin_package()

################################################################################
# Install
################################################################################

foreach(dir config launch)
  install(DIRECTORY ${dir}
          DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
endforeach(dir)
