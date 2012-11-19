cmake_minimum_required(VERSION 2.8.3)
project(sbox3)

find_package(catkin REQUIRED sbox2)

catkin_package(
  DEPENDS sbox2)

include_directories(include ${catkin_INCLUDE_DIRS})
add_executable(sbox3 sbox3.cpp)
target_link_libraries(sbox3 sbox2)
