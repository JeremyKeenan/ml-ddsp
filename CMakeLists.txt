# CMakeLists.txt

cmake_minimum_required(VERSION 3.0)
project(ml-ddsp)

# Specify available architectures
if(APPLE)
    set(CMAKE_OSX_ARCHITECTURES "x86_64;arm64")  # Allow both x86_64 and arm64
    # Other configurations as needed
endif()

# Add other necessary CMake configurations and targets...