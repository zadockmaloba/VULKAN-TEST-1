cmake_minimum_required(VERSION 3.0)

project(vulkan_test1)

find_package(Vulkan REQUIRED)
find_package(glfw3 REQUIRED glfw3)

add_executable(vulkan_test1 main.cpp)

target_link_libraries(vulkan_test1 ${VULKAN_LIB_LIST}
-lglfw -lvulkan -ldl -lpthread -lX11 -lXrandr -lXi
)

install(TARGETS vulkan_test1 RUNTIME DESTINATION bin)
