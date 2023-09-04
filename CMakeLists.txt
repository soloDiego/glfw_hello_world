cmake_minimum_required(VERSION 3.27.0)
project(glfw_hello_world VERSION 0.1.0)

find_package(OpenGL REQUIRED)

add_executable(glfw_hello_world 
    src/main.cpp
    src/glad.h
    src/glad.c
)

target_link_libraries(glfw_hello_world 
    glfw
    GL
)