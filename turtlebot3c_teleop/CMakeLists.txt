################################################################################
# Set minimum required version of cmake, project name and compile options
################################################################################

cmake_minimum_required(VERSION 2.8.3)
project(turtlebot3c_teleop)

################################################################################
# Install
################################################################################

foreach(dir config launch)
  install(DIRECTORY ${dir}/
          DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/${dir})
endforeach(dir)
