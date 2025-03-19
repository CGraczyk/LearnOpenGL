cmake_minimum_required(VERSION 3.10)
project(LearnOpenGL)

set(CMAKE_CXX_STANDARD 17)

# GLFW
add_subdirectory(external/glfw)
include_directories(external/include)

# GLAD
add_library(glad STATIC external/src/glad.c)
target_include_directories(glad PUBLIC external/include)

# OpenGL
find_package(OpenGL REQUIRED)

# Executable
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR})
add_executable(${PROJECT_NAME} hello_window.cpp)

# Link Libraries
target_link_libraries(${PROJECT_NAME} glfw glad OpenGL::GL)
