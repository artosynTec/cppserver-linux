cmake_minimum_required(VERSION 3.5.1)
project(cppserver_linux)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11  -pthread")

aux_source_directory(./src DIR_SRCS)

add_executable(cppserver_linux src/main.cpp ${DIR_SRCS})
