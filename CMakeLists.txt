#  CMakeLists.txt

cmake_minimum_required(VERSION 3.0)

# Set project name and type
project(ml-ddsp LANGUAGES CXX)

# Specify ARM64 architecture support
if(CMAKE_SYSTEM_PROCESSOR MATCHES "arm64")
    message(STATUS "Building for ARM64 architecture")
else()
    message(ERROR "Unsupported architecture.")
endif()

# Include additional directories or libraries if needed
include_directories(include)

# Add your source files here
set(SOURCES
    src/main.cpp
    src/utils.cpp
)

add_executable(ml-ddsp ${SOURCES})
