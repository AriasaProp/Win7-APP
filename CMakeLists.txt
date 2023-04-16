cmake_minimum_required (VERSION 3.10)

project(Win7-App LANGUAGES CXX)

set(CMAKE_BUILD_TYPE Release)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSION OFF)
set(CMAKE_GENERATOR_PLATFORM Win32)

# Add the include directory
file(GLOB_RECURSE Include_Dir LIST_DIRECTORIES true ".")
file(GLOB_RECURSE Src_Files "*.cpp")

include_directories(${Include_Dir})
# Add the executable
add_executable(${PROJECT_NAME} ${Src_Files})
