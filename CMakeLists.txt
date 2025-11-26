cmake_minimum_required(VERSION 3.10)
project(MLAT_SIMULATION CXX)

find_package(Eigen3 REQUIRED)

include_directories(${EIGEN3_INCLUDE_DIR})

add_executable(mlat_sim mlat_core.cpp mlatcpp_din5.cpp)
