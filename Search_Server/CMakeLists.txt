# Set cmake version
cmake_minimum_required(VERSION 3.11)

# Set the project name
project(SearchServerProject)

# Specify the C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Include directories
include_directories(include)

# Source files
set(SOURCES
    src/document.cpp
    src/main.cpp
    src/read_input_functions.cpp
    src/request_queue.cpp
    src/search_server.cpp
    src/string_processing.cpp
)

# Add the executable
add_executable(SearchServer ${SOURCES})
