cmake_minimum_required(VERSION 2.8.3)
project(dreamer)


## Find catkin macros and libraries
## if COMPONENTS list like find_package(catkin REQUIRED COMPONENTS xyz)
## is used, also find other catkin packages
find_package(catkin REQUIRED COMPONENTS roscpp)

# find_package(gazebo REQUIRED)

###################################
## catkin specific configuration ##
###################################
## The catkin_package macro generates cmake config files for your package
## Declare things to be passed to dependent projects
## INCLUDE_DIRS: uncomment this if you package contains header files
## LIBRARIES: libraries you create in this project that dependent projects also need
## CATKIN_DEPENDS: catkin_packages dependent projects also need
## DEPENDS: system dependencies of this project that dependent projects also need
catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES controlit
  CATKIN_DEPENDS roscpp
#  DEPENDS system_lib
)

# #set the default path for built executables to the "bin" directory
# set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
# #set the default path for built libraries to the "lib" directory
# set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)

#uncomment if you have defined messages
#rosbuild_genmsg()
#uncomment if you have defined services
#rosbuild_gensrv()

#common commands for building c++ executables and libraries
#rosbuild_add_library(${PROJECT_NAME} src/example.cpp)
#target_link_libraries(${PROJECT_NAME} another_library)
#rosbuild_add_boost_directories()
#rosbuild_link_boost(${PROJECT_NAME} thread)
#rosbuild_add_executable(example examples/example.cpp)
#target_link_libraries(example ${PROJECT_NAME})

# include (FindPkgConfig)
# if (PKG_CONFIG_FOUND)
#   pkg_check_modules(GAZEBO gazebo REQUIRED)
# else()
#   message(FATAL_ERROR "pkg-config is required; please install it")
# endif()

# message(STATUS ${GAZEBO_INCLUDE_DIRS})
# message(STATUS ${GAZEBO_LIBRARY_DIRS})

include_directories(
    # ${GAZEBO_INCLUDE_DIRS}
    ${catkin_INCLUDE_DIRS}
)

# if(CMAKE_COMPILER_IS_GNUCXX)
#     set(CMAKE_CXX_FLAGS "-std=c++0x ${CMAKE_CXX_FLAGS}")
# endif()

# include_directories(${GAZEBO_INCLUDE_DIRS})
# link_directories(${GAZEBO_LIBRARY_DIRS})

# add_library(dreamer_slave_joint_plugin 
#     gazebo_plugins/src/dreamer_slave_joint_plugin.cpp
# )

# target_link_libraries(dreamer_slave_joint_plugin 
#     ${GAZEBO_LIBRARIES}
# )

# add_library(dreamer_eye_plugin 
#     gazebo_plugins/src/dreamer_eye_plugin.cpp
# )

# target_link_libraries(dreamer_eye_plugin 
#     ${GAZEBO_LIBRARIES}
# )

# add_library(dreamer_pr2_gripper_plugin
#     gazebo_plugins/src/dreamer_pr2_gripper_plugin.cpp
# )

# target_link_libraries(dreamer_pr2_gripper_plugin 
#     ${GAZEBO_LIBRARIES}
# )
