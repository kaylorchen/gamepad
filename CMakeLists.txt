cmake_minimum_required(VERSION 3.22)
project(gamepad)

set(CMAKE_VERBOSE_MAKEFILE OFF)
set(CMAKE_CXX_STANDARD 14)

include_directories(drivers)
add_subdirectory(drivers)
add_executable(gamepad main.cpp)
target_link_libraries(gamepad f710)

