cmake_minimum_required(VERSION 3.1)
project (OpenGLPractice)

# Cmake Configuration #

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS}")

set(EXECUTABLE_OUTPUT_PATH "${CMAKE_BINARY_DIR}/bin")
set(glm_DIR /home/rohan/glm/cmake/glm)

# OpenGL Configuration #

find_package(OpenGL REQUIRED)
find_package(glm REQUIRED)

# Includes #

include_directories(${OPENGL_INCLUDE_DIR} ${GLM_INCLUDE_DIR})

add_subdirectory(src)
