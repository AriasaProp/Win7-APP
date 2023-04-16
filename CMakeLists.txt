cmake_minimum_required (VERSION 3.10)

project(Win7-App LANGUAGES CXX)

set(CMAKE_BUILD_TYPE Release)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSION OFF)
# Set the target platform to 32-bit
set(CMAKE_GENERATOR_PLATFORM Win32)

# Add the include directory
include_directories(include)
# Add the source directory
add_subdirectory(src)

# Add the executable
add_executable(my_project ${MY_SOURCES})
