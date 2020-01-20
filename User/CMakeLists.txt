cmake_minimum_required(VERSION 3.14)
set(CMAKE_CXX_STANDARD 14)

project(GreetTest)
set(SRC main.cpp)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
link_directories(${CMAKE_CURRENT_SOURCE_DIR}/lib)

add_executable(GreetTest ${SRC})
target_link_libraries(GreetTest PUBLIC Greeter)