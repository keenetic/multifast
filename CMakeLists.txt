cmake_minimum_required(VERSION 3.20)

project("multifast_examples" VERSION 0.1.0)

set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED ON)

option(MF_VERSION_NUMBER "Version number of multifast" "2.0.0")

set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fPIC -DMF_VERSION_NUMBER=${MF_VERSION_NUMBER}")

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/ahocorasick)
