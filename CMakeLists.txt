cmake_minimum_required(VERSION 3.5)

set(CMAKE_EXPORT_COMPILE_COMMANDS true)

set(CMAKE_CXX_FLAGS "-Wall -std=c++17")
set(CMAKE_CXX_FLAGS_DEBUG "-O0 -ggdb")

project (genGraph)


add_executable(${PROJECT_NAME} main.cpp)
if (CMAKE_BUILD_TYPE STREQUAL "Debug")
    message(STATUS "Build type: ${CMAKE_BUILD_TYPE}")
endif (CMAKE_BUILD_TYPE STREQUAL "Debug")

if (CMAKE_BUILD_TYPE STREQUAL "Release")
    message(STATUS "Build type: ${CMAKE_BUILD_TYPE}")
endif (CMAKE_BUILD_TYPE STREQUAL "Release")
