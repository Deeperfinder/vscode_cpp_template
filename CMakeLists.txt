cmake_minimum_required(VERSION 3.0.0)
project(yolo VERSION 0.1.0 LANGUAGES C CXX)

include(CTest)
enable_testing()
set(CMAKE_BUILD_TYPE "Debug")
add_executable(yolo main.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
