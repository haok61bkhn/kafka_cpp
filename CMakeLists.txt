set(PROJECT kafka)
project(${PROJECT} C CXX)
cmake_minimum_required(VERSION 2.8.11)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -Wextra -pedantic")

add_subdirectory(src)