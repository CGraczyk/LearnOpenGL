# LearnOpenGL

## Introduction
This is a simple starter project to open a window using OpenGL in VSCode. Follow the tutorials on [LearnOpenGL](https://learnopengl.com).

## Prerequisites
List of software and tools required to run the project:
* Visual Studio Code
* CMake
* OpenGL
* GLFW
* GLAD

## Installation
Steps to install the necessary dependencies:
1. Install Visual Studio Code from [here](https://code.visualstudio.com/).
2. Install CMake from [here](https://cmake.org/download/).
3. Download and integrate GLFW by cloning GLFW into your project:
    ```
    cd LearnOpenGL/external
    git clone https://github.com/glfw/glfw.git
    ```
4. Download GLAD from [here](https://glad.dav1d.de/) by setting the language to C/C++, GL version to 3.3 or above, profile to core, and leaving extensions empty. Press generate, download the .zip, and copy the include and src directories into `LearnOpenGL/external`.

## Running the Project
Steps to build and run the project (on Windows):
1. Build the project:
    ```
    cmake -S . -B build
    cmake --build build
    ```
2. Run the executable:
    ```
    .\build\Debug\LearnOpenGL.exe
    ```
