# i stole this from somewhere sorry
cmake_minimum_required(VERSION 2.8)
project(arrays)
set(CMAKE_BUILD_TYPE Release)
find_package(JNI REQUIRED)
include_directories(${JNI_INCLUDE_DIRS})
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
set(SOURCE_FILES UnsafeMemory.cpp UnsafeMemory.h)
add_library(arrays SHARED ${SOURCE_FILES})