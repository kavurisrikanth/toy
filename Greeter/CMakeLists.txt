cmake_minimum_required(VERSION 3.14)

project(Greeter)
set(CMAKE_CXX_STANDARD 14)

set(SRC main.cpp)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)

add_library(Greeter STATIC ${SRC})