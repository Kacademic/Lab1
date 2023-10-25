cmake_minimum_required(VERSION 3.0)

project(HelloWorld VERSION 1.0)

add_executable(hello_world src/hello.cpp src/name.cpp)
target_include_directories(hello_world PRIVATE include)
