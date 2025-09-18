cmake_minimum_required(VERSION 3.10)
project(cmakedemo C)

# Set C standard
set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED ON)

# Include directories
include_directories(${CMAKE_SOURCE_DIR}/include)

# Source files
set(SOURCES
    source/main.c
    source/io_utils.c
    source/math_utils.c
)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/build)

# Create executable
add_executable(main ${SOURCES})

# Set output directory for the executable
