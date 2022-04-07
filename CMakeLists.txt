cmake_minimum_required(VERSION 3.10)

# set the project name
project(Cmake-Armadillo)

# add the executable
add_executable(Cmake-Armadillo main.cpp)

find_package(Armadillo REQUIRED)
include_directories(${ARMADILLO_INCLUDE_DIRS})
target_link_libraries(Cmake-Armadillo ${ARMADILLO_LIBRARIES})
