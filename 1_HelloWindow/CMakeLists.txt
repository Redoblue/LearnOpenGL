cmake_minimum_required(VERSION 3.10) 

# set the project name 
project(1_HelloWindow)


include_directories(../0_common/glfw/3.3.2/include) 
include_directories(../0_common/glad/include)

link_directories(../0_common/glfw/3.3.2/lib)

add_executable(${PROJECT_NAME} main.cpp ../0_common/glad/src/glad.c)

target_link_libraries(${PROJECT_NAME} libglfw.dylib)