cmake_minimum_required(VERSION 2.8.3)
project(sbox2)

find_package(catkin REQUIRED sbox1)

catkin_package(
  INCLUDE_DIRS include
  LIBRARIES ${PROJECT_NAME}
  DEPENDS sbox1)

include_directories(include ${catkin_INCLUDE_DIRS})
add_library(${PROJECT_NAME} SHARED sbox2.cpp)

