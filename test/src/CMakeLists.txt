cmake_minimum_required(VERSION 3.5)
set(CMAKE_CXX_STANDARD 17)

add_executable(cpputil_test test.cpp)

target_link_libraries(cpputil_test gtest gtest_main)
include_directories(${PROJECT_SOURCE_DIR}/include)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fopenmp -march=native -O0")