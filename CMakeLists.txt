cmake_minimum_required(VERSION 3.0)

project(vulkan_test1)

add_executable(vulkan_test1 main.cpp)

install(TARGETS vulkan_test1 RUNTIME DESTINATION bin)
