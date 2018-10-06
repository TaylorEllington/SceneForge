cmake_minimum_required(VERSION 3.5)
project(SceneForge VERSION 0.1 LANGUAGES CXX)

set(BUILD_SUPPORT_DIR ${CMAKE_SOURCE_DIR}/build-support)
set(LIB_DIR ${CMAKE_SOURCE_DIR}/lib)

set(CMAKE_MODULE_PATH  ${BUILD_SUPPORT_DIR})


add_subdirectory(third-party)
add_subdirectory(src)